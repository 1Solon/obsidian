![[Pasted image 20240129151719.png]]
> * Developed at Stanford University in the 80’s * The V operating system (sometimes written V- System) is a microkernel operating system * The key concepts in V are multithreading and synchronous message passing. « Communication between threads in V uses synchronous message passing, with short, fixed- length messages that can include access rights for the receiver to read or write part of the sender's address space before replying

![[Pasted image 20240129151739.png]]
> * One common pattern for using the messaging facility is for clients to send messages to a server requesting some form of service. * This is similar to modern-day Remote Procedure call RPC

## Impacts of V
---
![[Pasted image 20240129151800.png]]
> After the initial implementation on a single computer, a protocol called the Versatile Message Transaction Protocol (VMTP) was developed to extend the send-receive-reply system call semantics over a local area network The protocol included multicast support developed by Steve Deering as a graduate student in the group. * The Internet Protocol layer to support this evolved into the IP multicast standard

## V and Gui
---
![[Pasted image 20240129151818.png]]
> * The Virtual Graphics Terminal Service (VGTS) provided a modular windowing system for both local and remote applications. * The little-known W Window System got its name because it was first hosted on the V operating system, and the better-known X Window System (Unix GUI) in turn got its name because its first version was based partly on W.