**Definition:**
![[Pasted image 20211007091712.png]]
* The server receives the client’s request, performs the necessary
computation and returns the result to the client.

* The server provides access to services or data on the server system

* While some services or data can be offered to anyone, some must be
kept secure

**Client Server Model Security:**
* Servers must contain code that handles the issues of
	* Authentication: Verify the Client identity.
	* Authorization: Is client permitted to access the service. Student and staff are authorized different role for web course
	* Data security: The protection of data from unauthorized access. 

**Links:**
* [[Sockets]]
* [[ipv4 header]]
* [[Type of Service in RFC791]]

## Visual Diagram:
![[Pasted image 20240102152353.png]]

## Alternate Explanation (From Systems Architectures)
---
![[Pasted image 20240122162249.png]]
> * Client-server model — defines roles for 2 interacting entities — client: * needs a particular service * sends request to server + gets (after some time) reply — server. » awaits requests from clients » performs requested function — server can be client of another server

![[Pasted image 20240122162413.png]]
> ® Clients send requests to servers (i.e., invocation) ® Servers send responses to clients (i.e., result) ® Servers may be clients of other servers - A web server is often a client of a file server — An Internet service is a client of a DNS server - a server that translates DNS names to IP addresses ® Potential problem: a single server is a scalability bottleneck and a single point of failure

### Alternative Diagram
---
![[Pasted image 20240122162317.png]]