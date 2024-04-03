## Q1: In this situation, what is a possible reason that causes a “Deadlock”?
A deadlock can occur in this situation if cars from all 4 directions try to cross the intersection at the same time.

## Q2: How to prevent from the Deadlock?
This deadlock could be prevented by simply adding a stop sign to at least one of the sides of the intersection.

## Q3: What are the differences between threads and child processes?
Unlike child processes, all threads in a process share data such as address space and global variables. They are also faster to create than child processes.

## Q4: What are the differences between multi-threads and multi-tasking?
Multi-threads mean a process has multiple threads and multi-tasking means for example your cpu has multiple cores and can run multiple processes at once.

## Q5: What digits in Base2 represent values 15 and 16 in Base10?
001111 = 15
010000 = 16

## Q6: Is 64-bit system better than 32-bit system? Why?
Yes, because a 64 bit system can handle bigger numbers and thus can handle more complex and larger operations.

## Q7: How many bits represent 1 byte of memory? When to use Bits and when to use Bytes?
8 bits is 1 byte of memory. Bits are used when we are talking about individual base 2 values and bytes are used when storing letters and such.

## Q8: What happens if your computer has more than “4GB” memory but it runs a “32-bit Windows”?
Windows will fail to recognize any more than 4GB of it

## Q9: What are RAM and ROM?
RAM is volatile memory that is super fast and is wiped when the computer is turned off. ROM is non-volatile memory and is slower but does not get wiped when the computer is turned off.

## Q10: Why does a system need to have RAM? What happens if a system has no RAM?
A system needs RAM to store information required for the execution of an OS as well as processes running in the OS. A system without RAM cannot boot.

## Q11: How the address of a process is used?
A memory address of a process is used not only to locate the process and all code that goes along with it but it also provides a base and limit so that the OS knows how much RAM is free and the process has boundaries as to what resources it can use.

## Q12: Why are “binary digits” not good for writing an address of a memory?
Binary digits are long and also harder to read compared to hex values.

## Q13: How many binary digits equal to one hex digit?
4

## Q14: Can a software recognise “physical address” ? Why?
No, because not even the CPU can reconise physical memory addresses. Thats why we need the MMU

## Q15: Why could a single process be allocated with “non-continuous” pages of memory?
So that the OS can best maximize the amount of RAM available.

## Q16: What is the difference between Paging and Segmentation?
Pages are statically sized vs segmentation where segments are variable-sized.

## Q17: What are unusable memory fragments? What is a potential effect caused by them?
Unusable memory fragments are small parts of memory that are not usable because a process is too large or you are using external fragmentation. This means that the fragments must be contiguous.

## Q18: How can we solve the external fragmentation problem?
By using compaction, or compressing empty space around processes in memory.

## Q19: What should OS do if reallocating one process still does not provide enough free memory?
Reallocate other parts of the memory if possible or use internal fragmentation

## Q20: Can the internal fragmentation be solved by “reallocating” current processes?
No.

## Q21: Who is responsible for “reducing” the possibility of internal fragmentation problem?
The programmers behind a program are responsible for this.

## Q22: Why a single process could be allocated with “non-continuous” blocks of memory?
Can reduce internal fragmentation and memory wastage caused by internal and/or external fragmentation.

## Q23: What are the two types of “Fragmentation” problems?
Internal and External fragmentation problem

## Q24: What is the main benefit of using Virtual Memory? What is a possible drawback of VM?
Because ROM is normally much larger than RAM, you can gain much more RAM through this method however ROM is much slower then RAM so its not always the best option.

## Q25: Why do we need a memory swapping?
To free up space in the main memory to process currently running processes. Only completely idle processes can be stored in the ROM using this method.

## Q26: Why some pages need to be swapped out? Why some pages still “remain” in a memory?
Because the OS can predict what parts of a process are going to be used in the very near future

## Q27: Why is it not good to have unnecessary swapping?
This can put strain on both the CPU, RAM and ROM but also increases the chance of something going wrong in the swapping process.