	Process
	
	![[Pasted image 20240901155042.png]]
	![[Pasted image 20240901155056.png]]
	![[Pasted image 20240901155112.png]]

## PCB
	Process control block 
		aldo know as Task control Block 
		associated with every process 
		
	![[Pasted image 20240901165741.png]]
	![[Pasted image 20240901165813.png]]

## Threads 
	![[Pasted image 20240901165911.png]]
## Process Scheduling 
	Maximizes CPU usage, switcing to processess onto CPU for time sharing 
	Process scheduler => selects the process for next execution 
	Scheduling Queues 
		Job Q -> set of all processes in the system 
		Ready Q -> set of all processes residing inmain memory waiting for executing
		Device Q -> set of processes waiting for an IO device 
	Process migrated between these 

![[Pasted image 20240901170303.png]]

### Scheduler -> 
	Short-term scheduler  (or CPU scheduler) –
		selects which process should be executed next and allocates CPU
		Sometimes the only scheduler in a system
		Short-term scheduler is invoked frequently (milliseconds)  (must be fast)
	Long-term scheduler  (or job scheduler) –
		selects which processes should be brought into the ready queue
		Long-term scheduler is invoked  infrequently (seconds, minutes)  (may be slow)
		The long-term scheduler controls the degree of multiprogramming
	Processes can be described as either:
	I/O-bound process – spends more time doing I/O than computations, many short CPU bursts
	CPU-bound process – spends more time doing computations; few very long CPU bursts
	Long-term scheduler strives for good process mix

![[Pasted image 20240901170644.png]]
![[Pasted image 20240901172942.png]]
![[Pasted image 20240901173020.png]]
![[Pasted image 20240901173050.png]]
![[Pasted image 20240901173130.png]]
![[Pasted image 20240901173141.png]]
![[Pasted image 20240901173215.png]]
https://medium.com/@akshat.mistry/zombie-vs-orphan-process-21643ec75558
![[Pasted image 20240901173444.png]]
![[Pasted image 20240901173519.png]]
![[Pasted image 20240901173530.png]]
![[Pasted image 20240901173544.png]]
![[Pasted image 20240901174417.png]]
![[Pasted image 20240901174434.png]]
![[Pasted image 20240901174447.png]]
![[Pasted image 20240901174456.png]]
![[Pasted image 20240901174510.png]]
![[Pasted image 20240901174523.png]]
![[Pasted image 20240901174531.png]]
![[Pasted image 20240901174542.png]]


![[Pasted image 20240901185649.png]]![[Pasted image 20240901185700.png]]
