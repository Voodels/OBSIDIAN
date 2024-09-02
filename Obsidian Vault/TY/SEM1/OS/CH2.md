## Operating System Services ** imp
	UI 
		Almost all operating systems have a user interface (UI).
		Varies between Command-Line (CLI), Graphics User Interface (GUI),   Batch
	Program Execution 
		The system must be able to load a program into memory and to run that program, end execution, either normally or abnormally (indicating error)
	IO
		A running program may require I/O, which may involve a file or an I/O device
    File system manipulation 
	    The file system is of particular interest. Programs need to read and write files and directories, create and delete them, search them, list file Information, permission management.
	Communications –
		 Processes may exchange information, on the same computer or between computers over a network
		Communications may be via shared memory or through message passing (packets moved by the OS)
	Error detection –
		 OS needs to be constantly aware of possible errors
		May occur in the CPU and memory hardware, in I/O devices, in user program
		For each type of error, OS should take the appropriate action to ensure correct and consistent computing
		Debugging facilities can greatly enhance the user’s and programmer’s abilities to efficiently use the system
	Resource allocation - 
		When  multiple users or multiple jobs running concurrently, resources must be allocated to each of them
		Many types of resources -   CPU cycles, main memory, file storage, I/O devices
    Accounting - 
	    To keep track of which users use how much and what kinds of computer resources
    Protection and security - 
	    The owners of information stored in a multiuser or networked computer system may want to control use of that information, concurrent processes should not interfere with each other
		Protection involves ensuring that all access to system resources is controlled
		Security of the system from outsiders requires user authentication, extends to defending external I/O devices from invalid access attempts
		
	![[Pasted image 20240901150047.png]]

## System Calls ** imp
	
	![[Pasted image 20240901152236.png]]
	![[Pasted image 20240901152350.png]]
	![[Pasted image 20240901152426.png]]
	Often, more information is required than simply identity of desired system call
		Exact type and amount of information vary according to OS and call
	Three general methods used to pass parameters to the OS
		Simplest:  pass the parameters in registers
			 In some cases, may be more parameters than registers
		Parameters stored in a block, or table, in memory, and address of block passed as a parameter in a register 
			This approach taken by Linux and Solaris
		Parameters placed, or pushed, onto the stack by the program and popped off the stack by the operating system
		Block and stack methods do not limit the number or length of parameters being passed
## Types of System Calls 
	Process control
		create process, terminate process
		end, abort
		load, execute
		get process attributes, set process attributes
		wait for time
		wait event, signal event
		allocate and free memory
		Dump memory if error
		Debugger for determining bugs, single step execution
		Locks for managing access to shared data between processes
	File management
		create file, delete file
		open, close file
		read, write, reposition
		get and set file attributes
	Device management
		request device, release device
		read, write, reposition
		get device attributes, set device attributes
		logically attach or detach devices
	Information maintenance
		get time or date, set time or date
		get system data, set system data
		get and set process, file, or device attributes
	Communications
		create, delete communication connection
		send, receive messages if message passing model to host name or process name
			From client to server
		Shared-memory model create and gain access to memory regions
		transfer status information
		attach and detach remote devices
	Protection
		Control access to resources
		Get and set permissions
		Allow and deny user access

	#Example of SC
	
		![[Pasted image 20240901153013.png]]
			![[Pasted image 20240901153037.png]]
	![[Pasted image 20240901153255.png]]

System Programs
	File management -
		 Create, delete, copy, rename, print, dump, list, and generally manipulate files and directories
	Status information
		Some ask the system for info - date, time, amount of available memory, disk space, number of users
		Others provide detailed performance, logging, and debugging information
		Typically, these programs format and print the output to the terminal or other output devices
		Some systems implement  a registry - used to store and retrieve configuration information
	File modification
		Text editors to create and modify files
		Special commands to search contents of files or perform transformations of the text
	Programming-language support -
		 Compilers, assemblers, debuggers and interpreters sometimes provided
	Program loading and execution- 
		Absolute loaders, relocatable loaders, linkage editors, and overlay-loaders, debugging systems for higher-level and machine language
	Communications -
		 Provide the mechanism for creating virtual connections among processes, users, and computer systems
		Allow users to send messages to one another’s screens, browse web pages, send electronic-mail messages, log in remotely, transfer files from one machine to another
	Background Services
		Launch at boot time
			Some for system startup, then terminate
			Some from system boot to shutdown
		Provide facilities like disk checking, process scheduling, error logging, printing
		Run in user context not kernel context
		Known as services, subsystems, daemons 
	Application programs
		Don’t pertain to system
		Run by users
		Not typically considered part of OS
		Launched by command line, mouse click, finger poke

		![[Pasted image 20240901153706.png]]
		![[Pasted image 20240901153735.png]]
	![[Pasted image 20240901153850.png]]
	![[Pasted image 20240901153919.png]]
	