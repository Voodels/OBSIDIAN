## What is OS? 
	program acting as an intermeditary between a user and computer hardware 
	Operating system goals:
		Execute user programs and make solving user problems easier
		Make the computer system convenient to use
		Use the computer hardware in an efficient manner


## Computer System structure 
	Hardware -> Resources 
	OS -> control and cordination 
	application programs -> 
	Users-> 

	![[Pasted image 20240901141742.png]]

## OS definition 
	OS is a resource allocator
	Manages all resources
	Decides between conflicting requests for efficient and fair resource use
	OS is a control program
	Controls execution of programs to prevent errors and improper use of the compute

***The one program running at all times on the computer” is the kernel. ***

bootstrap -> bootloader -> loads up the kernel initilazizes all the aspects 
	$$An__operating__system_is_interrupt_driven$$
	![[Pasted image 20240901142524.png]]
	DMA -> data from buffer to main memory without CPU intervention 

## Operating System Structure 
	# Multiprogramming (Batch system)-> 
		Single user cannot keep CPU and I/O devices busy at all times
		Multiprogramming organizes jobs (code and data) so CPU always has one to execute
		A subset of total jobs in system is kept in memory
		One job selected and run via job scheduling
		When it has to wait (for I/O for example), OS switches to another job
		
	Timesharing (multitasking) is logical extension in which CPU switches jobs so frequently that users can interact with each job while it is running, creating interactive computing
	Response time should be < 1 second
	Each user has at least one program executing in memory process
	If several jobs ready to run at the same time  CPU scheduling
	If processes don’t fit in memory, swapping moves them in and out to run
	Virtual memory allows execution of processes not completely in memory
## 
![[Pasted image 20240901143225.png]]

## Process Management 
	![[Pasted image 20240901143343.png]]
	Creating and deleting both user and system processes
	Suspending and resuming processes
	Providing mechanisms for process synchronization
	Providing mechanisms for process communication
	Providing mechanisms for deadlock handling
![[Pasted image 20240901143600.png]]


![[Pasted image 20240901143829.png]]

![[Pasted image 20240901143923.png]]
![[Pasted image 20240901143939.png]]
![[Pasted image 20240901144123.png]]
![[Pasted image 20240901144247.png]]

DATA STRUCTURES USED IN OS -> KERNEL 
	SLL DLL CLL 
	BST 
	BITMAP HASH 
	![[Pasted image 20240901144440.png]]
	![[Pasted image 20240901144515.png]]
	