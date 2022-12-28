Interrupts to the [[zk/CPU]] are issued by a device or program and depending on their priority will delay the execution of the currently running program until they are completed. Interrupts are issued on the Control Bus and the Program Counter of the previously executing program(s) is stored in a stack register.

[Craig'n'Dave Video](https://www.youtube.com/watch?v=PCYI1o592dQ) covering the basics

## Hardware Interrupts
- Memory Party Errors
- Power/Reset buttons

## Software Interrupts
- Illegal Operations
- User
- Logon/Authentication Request

## I/O
- Buffer (to drive, printer, etc) run/nning out of space
- Data operation completed (move/copy)