![[Pasted image 20240129151912.png]]
> * VMScluster is a computer cluster involving a group of computers running the OpenVMS operating system. * Whereas tightly coupled multiprocessor systems run a single copy of the operating system, a VMScluster is loosely coupled: each machine runs its own copy of OpenVMS, but the disk storage, lock manager, and security domain are all cluster-wide. * Machines can join or leave a VMScluster without affecting the rest of the cluster.

![[Pasted image 20240129151924.png]]
> * Interesting feature is the Disk Controller * Processes can share a set of disks * Access to disks is then co-ordinated between processes * All systems run VMS operating system