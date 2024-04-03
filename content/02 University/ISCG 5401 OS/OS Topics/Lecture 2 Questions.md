# Q1: What is the purpose of system calls
A1: A system call acts as an interface between a program running in the user space and the OS. These calls are used to request services and functions from the OS's kernel

# Q2: What is the purpose of the command interpreter? Why is it usually separate from the kernel?
A2: The main role of the command interpreter is to read, interpret and execute commands that are either entered by a user or called upon by a program. The command interpreter is usually separate from the kernel for multiple reasons. Some of these include,
- Security
- Speed and
- Flexibility

# Q3: What is the purpose of system programmes?
A3: System programmes provide basic functionality to users so that users do not need to reinvent the wheel to achieve common tasks.

# Q4: What is the main advantage and disadvantages of the layered approach to system to system designs?
A4: The system is very easy to debug, if another service crashes you can debug that rather than restarting the whole system. Having a layered approach makes the system very secure.