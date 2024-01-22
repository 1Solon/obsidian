![[Pasted image 20210927113652.png]]
**General Notes:**
* Amazon Virtual Private Cloud (Amazon VPC) is a service that lets you provision a logically isolated section of the AWS Cloud (called a virtual private cloud, or VPC) where you can launch your AWS resources.

* Amazon VPC gives you control over your virtual networking resources, including the selection of your own IP address range, the creation of subnets, and the configuration of route tables and network gateways. You can use both IPv4 and IPv6 in your VPC for secure access to resources and applications.

* You can also customize the network configuration for your VPC. For example, you can create a public subnet for your web servers that can access the public internet. You can place your backend systems (such as databases or application servers) in a private subnet with no public internet access.

* Finally, you can use multiple layers of security, including security groups and network access control lists (networkACLs), to help control access to Amazon Elastic Compute Cloud (Amazon EC2) instances in each subnet.

* [[VPC Security]]

![[Pasted image 20210927113843.png]]
**VPC and Subnets:**
* Amazon VPC enables you to provision virtual private clouds (VPCs). A VPCis a virtual network that is logically isolated from other virtual networks in the AWS Cloud. A VPC is dedicated to your account. VPCs belong to a single AWS Region and can span multiple Availability Zones.

* After you create a VPC, you can divide it into one or more subnets. A subnetis a range of IP addresses in a VPC. Subnets belong to a single Availability Zone. You can create subnets in different Availability Zones for high availability. Subnets are generally classified as public or private. Public subnets have direct access to the internet, but private subnetsdo not.

![[Pasted image 20210927114125.png]]
**VPC IP's:**
* IP addresses enable resources in your VPC to communicate with each other and with resources over the internet. When you create a VPC, you assign an IPv4 CIDR block (a range of privateIPv4 addresses) to it. After you create a VPC, you cannot change the address range, so it is important that you choose it carefully. The IPv4 CIDR block might be as large as /16 (which is 216, or 65,536 addresses) or as small as /28 (which is 24, or 16 addresses).

* You can optionally associate an IPv6 CIDR block with your VPC and subnets, and assign IPv6 addresses from that block to the resources in your VPC. IPv6 CIDR blocks have a different block size limit. 

* The CIDR block of a subnet can be the same as the CIDR block for a VPC. In this case,the VPC and the subnet are the same size (a single subnet in the VPC). Also, the CIDR block of a subnet can be a subset of the CIDR block for the VPC. This structure enables the definition of multiple subnets. If you create more than one subnet in a VPC, the CIDR blocks of the subnets cannot overlap. You cannot have duplicate IP addresses in the same VPC.

* Additional documentation availible here: (https://docs.aws.amazon.com/vpc/latest/userguide/vpc-ip-addressing.html)

![[Pasted image 20210927115115.png]]
**Reserved VPC IP:**
![[Pasted image 20210927115128.png]]
* The "Future Use" part of the domain can be user defined and used by a AWS user

**Public VPC IP:**
![[Pasted image 20210927115159.png]]

**Elastic VPC IP:**
![[Pasted image 20210927115219.png]]

**Route Tables:**
![[Pasted image 20211004094900.png]]

**Internet Gateway:**
![[Pasted image 20211004095009.png]]

**Internet Gateway (NAT)**
![[Pasted image 20211004095051.png]]
* A network address translation (NAT) gatewayenables instances in a private subnet to connect to the internet or other AWS services, but prevents the internet from initiating a connection with those instances.

* To create a NAT gateway, you must specify the public subnet in which the NAT gateway should reside. You must also specify an Elastic IP address to associate with the NAT gateway when you create it. After you createa NAT gateway, you must update the route table thatis associated with one or more of your private subnets to point internet-bound traffic to the NAT gateway. Thus, instances in your private subnets can communicate with the internet.

* You can also use a NAT instance in a public subnet in your VPC instead of a NAT gateway. However, a NAT gateway is a managed NAT service that provides better availability, higher bandwidth, and less administrative effort. For common use cases, AWS recommends that you use a NAT gateway instead of a NAT instance. 

**VPS Endpoints:**
![[Pasted image 20211004110752.png]]
* A VPC endpointis a virtual device that enables you to privately connect your VPC to supported AWS services and VPC endpoint services that are powered by AWS PrivateLink. Connection to these services does not require an internet gateway, NAT device, VPN connection, or AWS Direct Connect connection. Instances in your VPC do not require public IP addresses to communicate with resources in the service. Traffic between your VPC and the other service does not leave the Amazon network.

* An interface VPC endpoint(interface endpoint) enables you to connect to services that are powered by AWS PrivateLink. These services include some AWS services, services that are hosted by other AWS customers and AWS Partner Network (APN) Partners in their own VPCs (referred to as endpoint services), and supported AWS Marketplace APN Partner services. The owner of the service is the service provider, and you—as the principal who creates the interface endpoint—are the service consumer. You are charged for creating and using an interface endpoint to a service. Hourly usage rates and data processing rates apply.

* Gateway endpoints: The use of gateway endpoints incurs no additional charge. Standard charges for data transfer and resource usage apply. 