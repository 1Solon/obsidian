![[Pasted image 20240129144109.png]]
> Processes * A Process is a program in execution. It is a unit of work within the system * A Program is a passive entity- Dijkstra described it as a text which can evoke computation * A process is active within the system and needs resources to complete its task such as CPU , memory I/O files * Process termination releases resources

![[Pasted image 20240129144131.png]]
> Processes Continued * Typically system has many processes running concurrently on one or more CPUs * Processes can be whole i.e. single threaded or made up of different parts i.e. multi threaded. * Processes ,both system and user, compete for access to the CPU The CPU is timeshared amongst them according to some scheduling policy * Processes running on the CPU may be Interrupted.

## Process Management
---
![[Pasted image 20240129144610.png]]
> Process management activities * Creating and Deleting System and User Processes * Maintaining Lists of Processes + Suspending and resuming processes * Process scheduling * Process Synchronization * Process Communication ¢ Interrupt Handling * Deadlock Handling

## Interrupt Handling
---
* [[Interrupts]]