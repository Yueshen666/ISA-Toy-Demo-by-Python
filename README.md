# Basic ISA...

## machine models
Where does operand come from and where do results go?
The 3 most common types of ISAs are:
  1. Stack - The operands are implicitly on top of the stack.
  2. Accumulator - One operand is implicitly the accumulator.
  3. General Purpose Register (GPR) - All operands are explicitely mentioned, they are either registers or memory locations.
## Data Types(repr-operands) and Sizes 
1. Types: Binary integers, Binary coded decimals, floating point, packed vector data, (addresses)
2. Width: Binary integer (8-bit ~ 64bit),floating point(32,40,64,80bit),address(16bit,..64bit)
## Addressing Models(operands location)
How to get operands from memory? 
  1. Register
  2. Imm
  3. displayment
  4. absolute
  5. Register indirect
  6. mem indirect...
## Number of explicit named operands
...
## classes of instructions
1. Data Transfer: LD, ST..
2. ALU: ADD, SUB, AND, MUL, XOR...
3. Control flow: JR, TRAP...
4. Floating Point: ADD.D, MUL.D...
5. (Multimedia)
6. String: rep movesb
## ISA encoding
1. fixed length(every instruction has same length, easy to code): RISC: MIPS(all 4 bytes),powerpc, ARM
2. variable length: CISC: take less space in mem and caches: x86(from 1 - 17bytes)
## RISC
1. Reduced : the number of bits that are used for the opcode is reduced.
2. EX:MIPS, All ALU instructions have 3 operands which are only registers. The only memory access is through explicit LOAD/STORE instructions. 
Thus C = A + B will be assembled as:

`LOAD  R1,A`

`LOAD  R2,B`

`ADD   R3,R1,R2`

`STORE C,R3`

Please see [Ref](http://www.cs.kent.edu/~durand/CS0/Notes/Chapter05/isa.html)

# A Design
## General
## Registers
## Arithmetic instructions
## pipeline/solution to harzard/cache...
