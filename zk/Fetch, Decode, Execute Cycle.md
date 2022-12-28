# Fetch
The [[zk/CPU]] from the memory address stored in the [[zk/CPU#Program Counter]] using the [[zk/CPU#Address Bus]]

The contents of this memory address are then sent from memory (either [[zk/CPU#Registers]], [[zk/CPU#Cache]] or [[zk/RAM]]/[[zk/ROM]]) using the [[zk/CPU#Data Bus]] and stored in the [[zk/CPU#Accumulator]].

# Decode
The CPU translates the [[zk/Assembly#Opcodes]] to its corresponding action, for example reading from memory or performing an arithmetic operation.

# Execute
The CPU executes the instruction.
The output of [[zk/CPU#ALU]] operations or memory reads will be stored in the Accumulator.

We then return to the Fetch stage of the cycle