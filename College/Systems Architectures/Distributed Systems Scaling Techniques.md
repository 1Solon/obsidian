![[Pasted image 20240129155229.png]]
> * Scalability affects performance more than anything else. * Three techniques to improve scalability: — Hiding communication latencies — Distribution — Replication

![[Pasted image 20240129155250.png]]

![[Pasted image 20240129155327.png]]

![[Pasted image 20240129155559.png]]
> Third Scaling Technique - Replication * Replication: multiple identical copies of something — Replicated objects may also be distributed, but aren’t necessarily. * Replication — Increases availability — Improves performance through load balancing — May avoid latency by improving proximity of resource
## Distribution
---
![[Pasted image 20240129155305.png]]
> * Instead of one centralized service, divide into parts and distribute geographically * Each part handles one aspect of the job — Example: DNS namespace is organized as a tree of domains; each domain is divided into zones; names in each zone are handled by a different name server — WWW consists of many (millions?) of servers

