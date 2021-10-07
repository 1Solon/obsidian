**Definition:**
* Socket is a connection between two hosts.

* Sockets allow the programmer to treat a network connection as  just like reading and writing the data on files.

* Sockets hide the programmer from low-level details of the network,
such as error detection, packet sizes.

**Socket Operations:**
1. Connect to a remote machine
2. Send data
3. Receive data
4. Close a connection
5. Bind to a port
6. Listen for incoming data
7. Accept connections from remote machines on the bound port

**Standard Vs. Non-standard**
* Standard application services are those defined by TCP/IP

* They are assigned well-known, widely recognised protocol port identifiers

* Examples are TELNET, FPT, SMTP

* Other services are called non-standard application services

**Types of Client Server:**
![[Pasted image 20211007111425.png]]

**TCP Vs. UDP:**
![[Pasted image 20211007111452.png]]

**Creating a Simple Client and Server:**
* [[Creating a Simple Server]]
* [[Creating a Simple Client]]