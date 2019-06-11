# tlpi
the linux programming interface overview

- [x] BSD: Berkeley Software Distribution
- [x] Ken Thompson graduated at Berkeley university
- [x] 1969 the first implementation of UNIX same year Linus Torvalds was born
- [x] OS do: managing, allocates resources and run software
- [x] functions: process scheduling, memory management, provisioning files system, creation and termination program, access to device, provisioning a system call application programming interface, networking
- [x] SUSv3: [-._a-zA-Z0-9] this is portable filename character set that recommend a file to follow when naming
- [x] the UNIX system have no term of end-of-file, the end of file is where a read that return no data
- [x] new line is a character(ASCII code: 10)
- [x] process is an instance of program
- [x] process divided into 4 segments: 
     - [x] text: the instruction of program
     - [x] data: the static variables used by the program
     - [x] heap: the area in which program can dynamically locate in extra memory
     - [x] stack: the piece of memory that grow and shrinks as function called and return and that is used to allocate storage for local variables and function call linkage information
 - [x] the process can create new process by using fork(), the new process refer as child process, the kernel create the child process by making duplicate of the parent process
 - [x] execve() (exec): system call to load and execute an entirely new program, this can destroy text, data stack and heap base on the code of new program
 - [x] the init process: first running process when system booting, which is have processID = 1 with root user. init process cannot be kill even root user, can only by terminate when system is shutdown.
 the main task is to create and monitor process that required for running system
 - [x] daemon is process that running when program start and terminate when system is shutdown,it running in background and dont need controlling terminal.
 - [x] environment list: a list of environment variables that maintained whithin user space memory.
 - [x] environment variable PATH: which is a list of directories that the shell should search when looking for programs corresponding to command enter by the user
 - [x] memory mapping(mmap()): use for allocate new zero-filled memory.
