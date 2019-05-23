# ALTARM-OS:

ALTARM-OS is an alternative operating system specifically designed for 
single board computers with the ARM CPU at there core.   That is the Clasic
ARM ISA (the standard 32-bit little endian ISA used by the ARMv1 through the ARMv7
[and available on early versions of the ARMv8]).

This is a desktop computer operating system, not to be confused with mobile device OS's.
I have used desktop computers running ARM CPU's for 30 years now, and it is still the
most reasonable CPU for desktop applicatioins out there.

# Features:
ALTARM-OS is a preemptive multitasking, protected memory, Microkernel, SMP capable, highly
modular Operating System, that already has a bunch of applications available to it (see next
section).

# API:

While it may have a different core structure and archetecture ALTARM-OS is going to be API
and binary compatible with RISC OS.   Thus the majority of existing RISC OS applications
should run on ALTARM-OS.   In other words ALTARM-OS is a true alternative Operating System
for ARM based computers, as RISC OS has long been the primary OS for ARM based systems
(many of the documents from ARM still include assembly language examples that only work on RISC OS).

So you will be able to run RISC OS applications in a true preemptive multitasking environment,
in fact all of the development of this OS, so far, is done in RISC OS and even some of the testing.

# Development:

This is a one man project so it will be slow.  I have a lot going with this operating system
already, though it is going to take a good bit more work to get something truely usable.

95% of the existing code is identicle between this and my other OS project for the ARM as the
other project is an API change from this one.

ALTARM-OS is written primarily in ARM Assembly language in a form that is compatible with AsAsm
and !ObjAsm on RISC OS.   I only use Linux to update these repos, and the releated documentation.

# Structure:

ALTARM-OS is much more modular than RISC OS, taking things that RISC OS grouped into single
modules, or crossed modules in awkward ways and splitting the modules better by functionality.

All modules except for the Kernel run in user mode, no more system mode access from module code
or user mode applciations.

I will be posting more information in the Wiki for this project as time progresses.


I am having some trouble at the moment uploading code to github, so there is an unwanted delay in posting the code I have.
