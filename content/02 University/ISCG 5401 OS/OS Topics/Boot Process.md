# About Booting:
Booting is the process of loading an operating system. It's the process that starts when we turn on the computer (using the power button or by a software command) and ends when the operating system is loaded into memory.

## Running BIOS:
When we turn on the computer, there is no programs inside the computer's main memory(RAM), so the CPU looks for another program, called the BIOS (Basic Input/Output System), and runs it. The BIOS is a firmware that is located on the motherboard and is run by the CPU to start the booting sequence.

## Running POST:
After the BIOS starts running, it starts a process called POST (Power-On Self-Test) which tests all the hardware devices and makes sure there are no issues. Moreover, if POST finds issues in the hardware, the booting process stops and the computer fails to boot.

## Loading MBR to RAM:
After running POST, the BIOS proceeds to load the MBR (Master Boot Record)