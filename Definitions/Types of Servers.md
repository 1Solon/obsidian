![[Pasted image 20211014113326.png]]

**Iterative:**
* Servers which handle one request at a time are called Iterative servers
* Iterative servers are easier to build and understand.
* They may have poor performance.

**Concurrent Servers:**
* Servers which handle more than one request at a time are called
Concurrent servers
* Concurrent servers can deliver better performance than Iterative
servers
* They require more programming effect as compare to Iterative
servers

**Connection-Orientated Servers:**
* A connection-oriented server uses the TCP transport protocol
* TCP handles errors, packet loss, and out-of-order delivery automatically for the application
* When the server connects to a client, TCP will deliver and receive all requests or responses or else inform the server that the connection has broken
* This simplifies the programming effort

**Connection less Servers:**
* A connection-less server uses the UDP transport protocol.
* Client or server must take responsibility for reliable delivery.
* UDP facilitates the multicast and broadcast communication