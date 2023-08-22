---
title: "ARM Architecture"
---
An architecture is defined by the instruction set and operand locations. It is based on the RISK (Reduced Instruction set computer) architecture and operates on **32-bit data**.

Each instruction in the computer is transmitted in machine language (pure binary), in ARM each instruction is a 32-bit word. We can use assembly language to understand these instructions.
![[Pasted images/Pasted image 20230726170319.png]]
A CPU is passed a binary program (sequence of instructions). The program counter is stored in a register and holds the current position in the program.
Even though ARM is a RISC architecture, not all instructions execute in a single processor cycle
## Memory
A matrix of storage elements that allows data to be written and read at specific addresses, and each address refers to a byte (8 bits) of data.
Even though data is byte addressed, CPUs can sometimes read/write more than 8-bits at a time – often referred to as a word.

Program memory is normally only read not written to. 
Data memory, memory that the program alters as a result of instructions being executed, is used for variables. 
Program and data memory can be physically different memory chips (Harvard Machine) or the same (Von Neumann Machine).
Instructions are fetched from memory at the current program counter.

![[Pasted images/Pasted image 20230726170757.png]]

## Coding Considerations:
- Strings in C are character arrays with “null termination” – a byte value of 0.
- C89 does not have built-in Boolean types, included in `stdbool.h`.
- use of `sizeof()`:
	- Allocated storage size for variable
	- `sizeof(unsigned char)` = 4
	- `sizeof(uint32_t)` = 4
	- `sizeof(_Bool)` = implementation specific
	- `sizeof(int)` = implementation specific 
	- `char data[40] `   `sizeof(data)` = 40
	- `char* ddata = data`;  ` sizeof(ddata)` = number of bytes to store a pointer (address, e.g. 32 bits)