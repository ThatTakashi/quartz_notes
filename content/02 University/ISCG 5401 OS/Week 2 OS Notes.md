# System Calls and System Programmes
- [[Registers vs RAM vs ROM]]
- [[Lecture 2 Questions]]
### System Calls
- A programmatic way in which a computer program requests a service from the kernel of the operating system
	- Hardware-related services
	- Creating and execution of new processes
	- communication with kernel services such as process scheduling
- System calls provide well-defined, safe implementations of operations
	- Instead of applications having direct access to system resources
- Most programming language provide a system call interface
	- It serves as the link to system calls available by the operating system
		- *Linux:* **PSOIX**
			- 300 different calls in Linux
		- *Windows:* **Win32**
			- 700 system calls in Windows 7

#### Types of System Calls
[[System calls]]
##### Process Control System Calls
- End, Abort, Load, Execute
- Create Process, Terminate Process
- Wait for time, Wait event, Signal event
- Allocate and free memory
- Locks for managing access to shared data between processes

##### File Management System Calls
- Create, Delete, Open and close file
- Read, Write
- Get and set file attributes

##### Device Management System Calls
- Request/Release device
- Read, Write, Reposition
- Get/Set device attributes

##### Information Maintenance System Calls
- Get time or date, set time or date
- Get system data, set system data
- Get and set process, file, or device attributes

##### Communications System Calls
- Create, Delete communication connection
- Send, recipe messages
- Transfer status information
- Attach and detach system drives

##### Protection System Calls
- Control access to resources
- Get, set permissions
- Deny access to files

# Operating System Structure
### MS-DOS
Was written to provide the most functionality in the least amount of space
- Is not divided into modules
- Has some structure, but interfaces and levels of functionality are not well separated

### UNIX
- Has limited structuring 
- Consists of two separable parts
	- System programmes
	- The kernel
		- Consists of everything
			- Below the system call interface, and
			- Above the physical hardware
		- Provides the file system, CPU scheduling, memory management, and other operating system functions
		- A large number of functions for one level

# System Boot
### System Programmes
System programmes provide a convenient environment for programme development and execution. Some of the tasks that these system programmes can help with are:
- File manipulation
- Programming language support
- Programme loading and execution
- Communications
- Background services

Most user's view of the operating system is defined by system programmes not the actual system calls.

#### Background Services
- Launch at boot time
	- Some for system startup, then terminate
		- Disk checking
	- Some for system boot and last till shutdown
		- Printer spooling
- Run in a user context not the kernel context
- Known as services, subsystems and daemons

### Application Programs (User Programs)
- Do not pertain to the system
- Are run by the user
- Not typically considered part of the OS
- Are launched via the command line or via a GUI with a mouse click or the tap of a finger