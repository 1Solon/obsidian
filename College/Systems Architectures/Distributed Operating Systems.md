![[Pasted image 20240129151141.png]]
> * The choice has traditionally been about centralized or different levels of distributed control- * When all resources local and remote managed centrally in the fashion of a single system operating system- These are known as Distributed Operating Systems * Alternatives are Networked operating Systems or cooperating peer to peer models

![[Pasted image 20240129151201.png]]
> * A distributed OS provides the same essential services and functionality required of an OS but adds attributes and particular configurations to allow it to support additional requirements such as increased scale and availability. * To a user, a distributed OS works in a manner similar to a single-node, monolithic operating system. That is, although it consists of multiple nodes, it appears to users and applications as a single-node.

![[Pasted image 20240129151609.png]]
> Early distributed systems emphasized the single system image — often tried to make a networked set of computers look like an ordinary general purpose computer * Examples: Amoeba, Sprite, NOW, Condor (distributed batch system), ...

## Abstractions Required in Distributed Operating Systems
---
![[Pasted image 20240129151233.png]]

## Networked Operating System
---
![[Pasted image 20240129151432.png]]
> * A looser more federated system is where nodes are largely autonomous with their own system but a central operating system manages shared resources and services for the network

![[Pasted image 20240129151443.png]]
> * An operating system oriented to computer networking, to allow shared file and printer access among multiple computers in a network, to enable the sharing of data, users, groups, security, applications, and other networking functions, typically over a local area network (LAN), or private network. * This sense is now largely historical, as common operating systems generally now have such features included.

## Cooperating between nodes in peer to peer networks
---
![[Pasted image 20240129151520.png]]
> * Cooperation varies according to whether the network is structured or unstructured * Unstructured peer-to-peer networks do not Impose a particular structure on the overlay network by design, but rather are formed by nodes that randomly form connections to each other.

## Structured Network
---
![[Pasted image 20240129151549.png]]
> * In structured peer-to-peer networks the overlay is organized into a specific topology, and the protocol ensures that any node can efficiently search the network for a file/resource, even if the resource is extremely rare. * The most common type of structured P2P networks implement a distributed hash table in which a variant of consistent hashing is used to assign ownership of each file to a particular peer

## Examples
---
* [[LOCUS]]
* [[Newcastle Connection]]
* [[The V System]]
* [[Amoeba]]
* [[VaxCluster]]