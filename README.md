# minix3
Studying the MINIX 3 operating system.

# Chapter 1 Questions

1. What are the two main functions of an operating system?

    * Extend the machine. Make it easier to program the underlying hardware.
    * Manage resources. Processors, memories, I?O devices, etc...

2. What is the difference between kernel mode and user mode?  Why is the difference important to an operating system?

    * Kernel mode: The operating system usually runs in the kernel mode.  It is protected from tampering by the hardware. System calls generally operate in kernel mode.
    * User mode: Programs written by the user run in user mode and are generally not protected by the hardware. Applications, editors, compilers, etc... run in user mode.
    * Importance: In order to remain stable and secure, the operating system needs to be protected from tampering, either inadverant or malicious.

3. What is multiprogramming?

    * Multiprogramming partitions memory into separate pieces so that one job can run in each memory space. When one job is idle, the CPU can run another job (in a partitioned memory space) and not worry about colliding with other jobs.

4. What is spooling? Do you think that advanced personal computers will have spooling as a standard feature in the future?

    * Spooling is Simultaneous Peripheral Operation On Line.  It allows a program to be read to disk in one of the memory partitions while another job is running.  That way, when a job was done, the "spooled" job would be ready to go and could start running immediately.  
    * To operate efficiently, I think some form of spooling will always be needed so that jobs can be ready to run when computing resources are available.  It may only be necessary for very compute-intensive programs which fully utilize computing resoureces and block other jobs from running.

5. On early computers, every byte of data read or written was directly handled by the CPU (i.e. there was no DMA - Direct Memory Access). What implications does this organization have for multiprogramming?

    * It would seem to indicate the jobs must all be loaded into memory prior to running the jobs to fully take advantage of multiprogramming.  Otherwise, the CPU would need to load the job into memory and this would block any jobs from running.

6. Why was timesharing not widespread on second-generation computers?

