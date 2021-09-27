![[Pasted image 20210927091626.png]]
**General notes:**
* Security and compliance are a shared responsibility between AWS and the customer. This shared responsibility model is designed to help relieve the customer’s operational burden. At the same time, to provide the flexibility and customer control that enables the deployment of customer solutions on AWS, the customer remains responsible for some aspects of the overall security. The differentiation of who is responsible for what is commonly referred to as security “of” the cloud versus security “in” the cloud.

**Responsibility:
* **AWS** operates, manages, and controls the components from the software virtualization layer down to the physical security of the facilities where AWS services operate. **AWS is responsible** for protecting the infrastructure that runs all the services thatare offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run the AWS Cloud services.
* **The customer is responsible** for the encryption of data at rest and data in transit. The customer should also ensure that the network is configured for security and that security credentials and logins are managed safely. Additionally, the customer is responsible for the configuration of security groups and the configuration of the operating system that run on compute instances that they launch (including updates and security patches).

![[Pasted image 20210927092015.png]]

**AWS Responsibility continued:**
* **Physical security of data centers** with controlled, need-based access; located in nondescript facilities, with 24/7 security guards; two-factor authentication; access logging and review; video surveillance; and disk degaussing and destruction.
* **Hardware infrastructure,** such as servers, storage devices, and other appliances that AWS relies on.
* **Software infrastructure,** which hosts operating systems, service applications, and virtualization software.
* **Network infrastructure,** such as routers, switches, load balancers, firewalls, and cabling. AWS also continuously monitors the network at external boundaries, secures access points, and provides redundant infrastructure with intrusion detection.

![[Pasted image 20210927092417.png]]

**Customer Responsibility Expanded:**
* While the cloud infrastructure is secured and maintained by AWS, customers are responsible for security of everything they put inthe cloud.
* ![[Pasted image 20210927092527.png]]
* Customers retain control of what security they choose to implement to protect their own data, environment, applications, IAM configurations, and operating systems.