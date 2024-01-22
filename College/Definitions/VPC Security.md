**General Notes:**
![[Pasted image 20211004111932.png]]
* A security groupacts as a virtual firewall for your instance, and it controls inbound and outbound traffic. Security groups act at the instance level, not the subnet level. Therefore, each instance in a subnet in your VPC can be assigned to a different set of security groups.

* At the most basic level, a security group is a way for you to filter traffic to your instances.

**Security Groups Continued:**
![[Pasted image 20211004112025.png]]
* Security groups have rulesthat control the inbound and outbound traffic. When you create a security group, it has no inbound rules. Therefore, no inbound traffic that originates from another host to your instance is allowed until you add inbound rules to the security group. By default, a security group includes an outbound rule that allows all outbound traffic. You can remove the rule and add outbound rules that allow specific outbound traffic only. If your security group has no outbound rules, no outbound traffic that originates from your instance is allowed

* Security groups are stateful, which means that state information is kept even after a request is processed. Thus,ifyou send a request from your instance, the response traffic for that request is allowed to flow in regardless of inbound security group rules. Responses to allowed inbound traffic are allowed to flow out, regardless of outbound rules.

**Custom Security Groups**
![[Pasted image 20211004112135.png]]
* When you create a custom security group, you can specify allow rules, but not deny rules. All rules are evaluated before the decision to allow traffic.

**Access Lists:**
![[Pasted image 20211004112324.png]]
* A network access control list (network ACL)is an optional layer of security for your Amazon VPC. It acts as a firewall for controlling traffic in and out of one or more subnets.To add another layer of security to your VPC, you can set up network ACLs with rules that are similar to your security groups.

* Each subnet in your VPC must be associated with a network ACL. If you don't explicitly associate a subnet with a network ACL, the subnet is automatically associated with the default network ACL. You can associate a network ACL with multiple subnets; however, a subnet can be associated with only one network ACL at a time. When you associate a network ACL with a subnet, the previous association is removed.

**Network Access Lists:**
![[Pasted image 20211004112420.png]]
* A network ACL has separate inbound and outbound rules, and each rule can either allow or deny traffic. Your VPC automatically comes with a modifiable default network ACL. By default, it allows all inbound and outbound IPv4 traffic and, if applicable, IPv6 traffic. The table shows a default network ACL.

* A network ACL has separate inbound and outbound rules, and each rule can either allow or deny traffic. Your VPC automatically comes with a modifiable default network ACL. By default, it allows all inbound and outbound IPv4 traffic and, if applicable, IPv6 traffic. The table shows a default network ACL.

**Custom Network Access Lists:**
![[Pasted image 20211004112520.png]]
* You can create a custom network ACL and associate it with a subnet. By default, each custom network ACL denies all inbound and outbound traffic until you add rules.

* A network ACL contains a numbered list of rules that are evaluated in order, starting with the lowest numbered rule. The purpose is to determine whether traffic is allowed in or out of any subnet that is associated with the network ACL. The highest number that you can use for a rule is 32,766. AWS recommends that you create rules in increments (for example, increments of 10 or 100) so that you can insert new rules where you need them later.

**Security Groups Versus Network ACLs:**
![[Pasted image 20211004112810.png]]
* Here is a summary of the differences between security groups and network ACLs:
	* Security groupsact at the instance level, but network ACLs act at the subnet level.
	* Security groups support allow rules only, but network ACLs support both allow and deny rules.
	* Security groups are stateful, but network ACLs are stateless.
	* For security groups, all rules are evaluated before the decision is made to allow traffic. For network ACLs, rules are evaluated in number order before the decision is made to alloxw traffic.



