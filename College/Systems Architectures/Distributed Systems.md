## What is a Distributed System?
---
![[Pasted image 20240122152732.png]]
> * A collection of independent computers that appears to its users as a single coherent system. * Features: — No shared memory — message-based communication — Each runs its own local OS — Heterogeneity * |deal: to present a single-system image: — The distributed system “looks like” a single computer rather than a collection of separate computers.

## Characteristics of a Distributed System
---
![[Pasted image 20240122152816.png]]
> * To present a single-system image: — Hide internal organization, communication details — Provide uniform interface * Easily expandable — Adding new computers is hidden from users ¢ Continuous availability — Failures in one component can be covered by other components * Supported by

![[Pasted image 20240129153608.png]]
> * Centralized: traditional client-server structure — Vertical (or hierarchichal) organization of communication and control paths (as in layered software architectures) — Logical separation of functions into client (requesting process) and server (responder) * Decentralized: peer-to-peer — Horizontal rather than hierarchical comm. and control — Communication paths are less structured; symmetric functionality * Hybrid: combine elements of C/S and P2P » Classification of a system as centralized or decentralized refers to communication and control organization, primarily.

## Goals of a Distributed System
---
![[Pasted image 20240122152854.png]]
> * Resource accessibility — For sharing and enhanced performance * Distribution transparency — For easier use * Openness — To support interoperability, portability, extensibility * Scalability — With respect to size (number of users), geographic distribution, administrative domains


## Advantages of Distributed Computing
---
![[Pasted image 20240129153851.png]]
> * Economics: better price/performance ratio: cost effective way to increase computing power. * Speed: a distributed system may have more total computing power than a mainframe. Enhanced performance through load distributing. * Inherent distribution: Some applications are inherently distributed. Ex. a supermarket chain. * Reliability: If one machine crashes, the system as a whole can still survive. Higher availability and improved reliability. * Incremental growth: Computing power can be added in small increments. Modular expandability

![[Pasted image 20240129153912.png]]
> * Data sharing: allow many users to access to a common data base * Resource Sharing: expensive peripherals like color printers * Communication: enhance human-to-human communication, e.g., email, chat * Flexibility: spread the workload over the available machines * Another driving force: the existence of large number of personal computers, the need for people to collaborate and share information.

## Issues of Distribution
---
![[Pasted image 20240122152926.png]]
> * Requirement for advanced software to realize the potential benefits. * Security and privacy concerns regarding network communication * Replication of data and services provides fault tolerance and availability, but at a cost. * Network reliability, security, heterogeneity, topology * Latency and bandwidth * Administrative domains

## Performance Advantages of Distributed Systems
---
![[Pasted image 20240129151957.png]]
> * Two performance advantages of distributed systems — Concurrently running components of applications. — Fewer users are competing for resources on different computers

## Challenges of Distributed Systems
---
* [[Heterogeneity]]
* [[Openess]]
* [[Security]]
* [[Scalability]]
* [[Failure Handling]]
* [[Concurrency]]
* [[Transparency]]


## Common Topologies
---
![[Pasted image 20240129153649.png]]
> * Four common topologies bus, ring, star, and tree. (Five, if you include the ‘hybrid’ topology.) * These topologies are logical architectures, but the hardware devices need not be physically organised in these configurations. Logical bus and ring topologies, for example, are commonly organised physically as a star.

![[Pasted image 20240129153713.png]]
![[Pasted image 20240129153734.png]]
* Star is the basis of [[Client Server Model]] 
* Star is the basis of message broker
* An example of this in use is a login server
* "Put key functionality in a central place, with no back up plan"
![[Pasted image 20240129153748.png]]
* Alternative to "ethernet" style topologies
* Commonly used in travel agents
* To communicate, you must "take ownership" of the ring
* This is accomplished with tokens and scheduling
![[Pasted image 20240129153805.png]]
* Hierarchical system
* "Head office, sub office, etc"
* "This kind of topology can develop naturally over time, as it follows what business often use"
* The problem is that it is prone to cascading failures
![[Pasted image 20240129153814.png]]
* Key goal is to provide multiple paths to each node
* Very failure tolerant
## Links
---
* [[Distributed Data Management]]
* [[Distributed Process Management]]
* [[Distributed Operating Systems]]
* [[Distributed Systems Scaling Techniques]]
* [[Data In Distributed Systems]]