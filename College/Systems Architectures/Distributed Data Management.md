![[Pasted image 20240129150614.png]]
> Data Distribution essentially involves *Centralized Data *Replicated Data *Partitioned data

## Centralised Data
---
![[Pasted image 20240129150638.png]]
> » User lists * Logins permission * Directory Single copy of the data at one location on the network * (Client Server Paradigm) * Easiest Maintenance * Least fault tolerance

## Replicated Data
---
![[Pasted image 20240129150705.png]]
> * Copies of the data are held at a subset of system nodes * Greater fault tolerance * Can actually be more efficient because of potential for parallel processing * Difficulty maintaining data consistency across all copies * Impacts updates , deletions, searches etc

![[Pasted image 20240129150727.png]]
> * Sophisticated protocols required + System admin more complicated

## Partitioned Data
---
![[Pasted image 20240129150747.png]]
> * Data is split up and parts deposited on different locations in memory * Merging parts is a key process * Finding all the parts and consistency is an issue * Dealing with local failure is an issue * Key question is whether to partition the directory or not

## Caching
---
* [[Caching Service]]

![[Pasted image 20240129150824.png]]
> * Caching is a form of replication — Normally creates a (temporary) replica of something closer to the user * Replication is often more permanent * User (client system) decides to cache, server system decides to replicate * Both lead to consistency problems