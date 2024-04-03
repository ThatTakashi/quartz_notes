### ALU
The Arithmetic and Logic Unit (ALU) preforms two types of operations:
- *Arithmetic operations* such as addition and subtraction
- *[[Logical operations]]* such as AND, OR, NOT and XOR

Its the CPUs calculator
The CU sends operations to the ALU
The ALU then takes the data

### FPU
The Maths coprocessor
- Preforms maths of *real numbers*
- Faster than the ALU for processing real numbers
- Standard CPU only works on integers
- The FPU uses special 80 bit registers

### Registers
Special *High speed* memory that is used by the CPU for the currently running task
- Memory scratchpad
- Temporary data storage space
- Register size (ie. 8bit, 16bit, 32bit, 64bit)
- The *word* size of a CPU - the number of bits that the CPU can handle at once
- Most *registers* are general purpose
	- Holds program data
- Some special registers
	- *Instruction Registers (IR)*
		- Contains the instruction the is currently being executed
	- *Instruction Pointers (IP)*
		- Points to the next instructions that the CPU is to execute

### The Accumulator

### Bus Interface Unit (BIU)
Connects the CPU to the bus on the motherboard
Connects the CPU to level 1, level 2 and level 3 cache
Contains *memory management unit (MMU)* which manages memory

*BSB (Back side bus)* = Internal Bus
*FSB (Front side bus)* = External Bus

### CU
The control unit (CU) controls and sequences the executions of instructions to the CPU
Then the CU makes sure that everything the CPU needs to do are done

#### CU Designs
- CISC
- RISC

### Cache
A small amount of super fast memory that is used to store frequently and recently used information

#### 3 levels
Level 1 Cache
Level 2 Cache
Level 3 Cache

Level 3 cache is the largest but slowest cache on the cpu, level 1 is the fastest but smallest on the other hand