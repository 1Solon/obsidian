* [[Distributed Data Management]]

![[Pasted image 20240129162111.png]]
> * Distributed Database: A single logical database that is spread physically across computers in multiple locations that are connected by a data communications link * Decentralized Database: A collection of independent databases on non-networked computers * Reference Chapter 13: Distributed Databases * Modern Database Management 7th Edition Jeffrey A. Hoffer, Mary B. Prescott, Fred R. McFadden * © 2005 by Prentice Hall

## Options (choose one of these)
---
![[Pasted image 20240129162132.png]]
> * Homogeneous - Same DBMS at each node — Autonomous - Independent DBMSs — Non-autonomous - Central, coordinating DBMS — Easy to manage, difficult to enforce * Heterogeneous - Different DBMSs at different nodes — Systems - With full or partial DBMS functionality — Gateways - Simple paths are created to other databases without the benefits of one logical database — Multidatabase * A multidatabase system (MDBS) is a facility that allows users access to data located in multiple autonomous database management systems (DBMSs). In such a system, global transactions are executed under the control of the MDBS. In- dependently, local transactions are executed under the control of the local DBMSs. — Difficult to manage, preferred by independent organizations

![[Pasted image 20240129162339.png]]
> * Data replication — Copies of data distributed to different sites * Horizontal partitioning — Different rows of a table distributed to different sites * Vertical partitioning — Different columns of a table distributed to different sites * Combinations of the above
## Control Options
---
* [[Federated]]
* [[Unfederated]]

## Distribution Options
---
* [[Replication]]
* [[Partitioning]]

## Five Distributed Database Organisations
---
![[Pasted image 20240129162705.png]]
> " Centralized database, distributed access " Replication with periodic snapshot update " Replication with near real-time synchronization of updates " Partitioned, one logical database " Partitioned, independent, nonintegrated segments

## Factors in Choice of Distributed Strategy
---
![[Pasted image 20240129162737.png]]
> * Funding, autonomy, security * Site data referencing patterns * Growth and expansion needs * Technological capabilities * Costs of managing complex technologies * Need for reliable service

## Distributed Design Matrix
---
![[Pasted image 20240129162813.png]]