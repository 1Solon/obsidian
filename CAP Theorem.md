![[Pasted image 20230926143757.png]]
> CAP Theorem = States that it is impossible for a distributed computer system to simultaneously provide all three of the following guarantees: = (Consistency (all nodes see the same data at the same time) ® This means that the data in the database remains consistent after the execution of an operation. For example after an update operation all clients see the same data. = All nodes show the same data at the same time = Availability (every request receives a response about whether it succeeded or failed) ® This means that the system is always on (service guarantee availability), no downtime. * Node failure does not stop other nodes = Partition tolerance (the system continues to operate despite arbitrary partitioning due to network failures) = this means that the system continues to function even when the communication among the servers is unreliable, i.e. the servers may be partitioned into multiple groups that cannot communicate with one another. = Arbitrary loss of messages does not cause failure (e.g. network failure) = Theoretically : Only 2 of the 3 are possible. = For NoSQL consistency is sacrificed


![[Pasted image 20230926144003.png]]
> CAP Theorem = CAP Theorem — 3 possible combinations = CA - Single site cluster, therefore all nodes are always in contact. When a partition occurs, the CAP Theorem system blocks. RDBMS CP - Some data may not be accessible, but the \CA CP/ E rest is still consistent/accurate. Partition AP Tolerance = AP - System is still available under partitioning, but some of the data returned may be . inaccurate.