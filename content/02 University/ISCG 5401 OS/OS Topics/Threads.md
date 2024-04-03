A **Thread** is the entity within a process that can be scheduled for execution. Processes are used to group resources together and threads are used to schedule program execution on the CPU.

- Consists of:
	- Thread ID
	- Program counter (register)
	- Stack
	- State
- All threads in a single process share
	- Address space
	- Global variables (files, child processes, accounting information)
	- Signals and signal handlers (alarms)

### Threads vs Child processes
Threads and child processes can look similar on the surface and they do largely share the same purpose and that is to break up tasks to complete them faster. There are a few differences between them and they are:
- Threads are faster to create than child processes and thus are more efficient
- Threads share code and resources unlike child processes

## Advantages of Multi-Thread
- **Responsiveness**
	- Allows a program to continue running even if part of it is blocked or preforming a lengthy operation (think of how a website loads when you open a web page)
	- Useful when creating programs in [[Code|programming]]
- **Resource Sharing**
	- Allows an application to have several different threads within the same address space