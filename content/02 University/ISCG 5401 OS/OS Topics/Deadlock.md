### What is a Process Deadlock
A situation in which two or more competing processes are each waiting for the other to finish, and thus neither ever does.

### What causes processes getting into a Deadlock?
- By resource (memory, I/O, Etc) sharing
	- Two or more processes trying to use the same resource

### Coffman Conditions
- If and only if all of these 4 conditions hold simultaneously causes a Deadlock
	- **Mutual Exclusion** (Mutex)
		- Only one process can use the resource at any given instance of time
	- **Hold and Wait** (Resource Holding)
		- A process is currently holding at least one resource and requesting additional resources which are being held by other processes
	- **No Pre-emption**
		- A resource can be released only voluntarily by the process holding it
	- **Circular Wait**
		- P1 must be waiting for a resource which is being held by P2, which in turn P2 is waiting for the first process to release the resource.
- These four conditions are known as the **Coffman Conditions**

### Deadlock Detection and Prevention
There are multiple algorithms for **pre-detection** of a possible Deadlock
- For example, removing the mutual exclusion condition means that no process will have exclusive access to a resource
	- Known as Non-blocking synchronization algorithms

### Deadlock Recovery
When a deadlock occurs, multiple processes get stuck waiting for each other to finish. If a deadlock occurs, the OS will attempt deadlock recovery. One of the easiest ways to fix a deadlock in the context of computer processes is to simply delete(or terminate) one or multiple processes such that other processes may complete their task.

Another solution may be to **roll-back**, but this can be difficult to manage if the queue is long.