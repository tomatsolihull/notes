# Direct Memory Access
![[attachments/Pasted image 20221105191528.png]]
From [this nice introduction video](https://youtu.be/M16l_ymlfcs)

## The Problem
When a [[zk/CPU]] wants to move a large amount of data to/from an I/O device into or out of memory, this process ties up the CPU and does not allow any other operations to take place. A transfer of every bit of data takes two CPU cycles to load and then store.

## The Solution
A DMA Controller is a simple processor that handles interfacing with I/O devices on behalf of the CPU.
The CPU tells the controller:
- whether the operation is read/write 
- the starting address of the I/O
- the starting address of the memory
- the size of the data block to transfer
An I/O device with its own DMA or a group of I/O devices on an I/O bus controlled by a DMA is able to only use one cycle to store the data.

## Cycle Stealing Process
Both the CPU and the DMA are on the same bus and cannot access it at the same time. This is called **bus contention**.
- DMA requests the bus (hold request)
- CPU acknowledges the request
  **Tri-Stating:** A third state beyond high/low or true/false. In this case it's **Z**, high-impedance. The CPU disconnects itself from the bus.
- The DMA takes control of the bus to transfer the data element
- The CPU is executing from its cache rather than the RAM so it can continue performing operations while the DMA has control of the bus. CPU only stalls if there is a cache miss while the DMA has control.

