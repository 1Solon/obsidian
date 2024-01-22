## What is a Distributed System?
---
![[Pasted image 20240122152732.png]]
> * A collection of independent computers that appears to its users as a single coherent system. * Features: — No shared memory — message-based communication — Each runs its own local OS — Heterogeneity * |deal: to present a single-system image: — The distributed system “looks like” a single computer rather than a collection of separate computers.

## Characteristics of a Distributed System
---
![[Pasted image 20240122152816.png]]
> * To present a single-system image: — Hide internal organization, communication details — Provide uniform interface * Easily expandable — Adding new computers is hidden from users ¢ Continuous availability — Failures in one component can be covered by other components * Supported by

## Goals of a Distributed System
---
![[Pasted image 20240122152854.png]]
> * Resource accessibility — For sharing and enhanced performance * Distribution transparency — For easier use * Openness — To support interoperability, portability, extensibility * Scalability — With respect to size (number of users), geographic distribution, administrative domains

## Issues of Distribution
---
![[Pasted image 20240122152926.png]]
> * Requirement for advanced software to realize the potential benefits. * Security and privacy concerns regarding network communication * Replication of data and services provides fault tolerance and availability, but at a cost. * Network reliability, security, heterogeneity, topology * Latency and bandwidth * Administrative domains

## Challenges of Distributed Systems
---
* [[Heterogeneity]]
* [[Openess]]
* [[Security]]
* [[Scalability]]
* [[Failure Handling]]
* [[Concurrency]]
* [[Transparency]]