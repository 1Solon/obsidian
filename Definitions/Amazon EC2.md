**General Notes:**
* [[EC2 Use Cases]]

**Launching an EC2 instance:**
![[Pasted image 20211011091822.png]]

* Amazon EC2 instancesrun as virtual machines on host computers that are located in AWS Availability Zones. Each virtual machine runs an operating system (OS), such as Amazon Linux or Microsoft Windows. You can install and run applications on the OS in each virtual machine. You can even run enterprise applications that span multiple virtual machines. 

* The virtual machines run on top of a hypervisorlayer that is maintained by AWS. The hypervisor is the operating platform layer that provides an EC2 instance with access to the actual physical hardware resources that it needs to run, such as processors, memory, and storage. 

* Some EC2 instances use an instance store. The instance store is also known as ephemeral storage. Itis storage that is physically attached to the host computer and provides temporary block-level storage to an instance. 

* Many EC2 instances use Amazon Elastic Block Store(Amazon EBS)for the boot disk and other storage needs. Amazon EBS provides persistent block storage volumes, which mean that the data will be persisted. For example, the data persists on that instance even when the EC2 instance is in a stopped state. 

* EBS-optimized instances provide faster access to an attached Amazon EBS volume by minimizing the I/O contention between the volume and other traffic from the instance.
