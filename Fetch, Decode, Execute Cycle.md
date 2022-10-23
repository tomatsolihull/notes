# Fetch
The [[CPU]] from the memory address stored in the [[CPU#Program Counter]] using the [[CPU#Address Bus]]

The contents of this memory address are then sent from memory (either [[CPU#Registers]], [[CPU#Cache]] or [[RAM]]/[[ROM]]) using the [[CPU#Data Bus]] and stored in the [[CPU#Accumulator]].

# Decode
The CPU translates the [[Assembly#Opcodes]] to its corresponding action, for example reading from memory or performing an arithmetic operation.

# Execute
The CPU executes the instruction.
The output of [[CPU#ALU]] operations or memory reads will be stored in the Accumulator.

We then return to the Fetch stage of the cycle