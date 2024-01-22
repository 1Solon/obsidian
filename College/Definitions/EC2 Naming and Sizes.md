![[Pasted image 20211011110406.png]]

* When youlook at an EC2 instance type, you will see that its name has several parts. For example, consider the T type.

* Tis the familyname, which is then followed by a number. Here, that number is 3.

* The number is the generationnumberof that type. So, a t3 instance is the thirdgeneration of the T family.In general, instance types thatare ofa higher generation are more powerful and provide a better value for the price.

* The next part of the name is the sizeportion of the instance. When you compare sizes, it is important to look at the coefficient portion of the size category.

* For example, a t3.2xlargehas twice the vCPU and memory of a t3.xlarge. The t3.xlarge has, in turn, twice the vCPU and memory of a t3.large.

* It is also important to note that network bandwidth is also tied to the size of the Amazon EC2 instance. If you will run jobs that will be very network-intensive, you might be required to increase the instance specifications to meet your needs