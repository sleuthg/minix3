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

