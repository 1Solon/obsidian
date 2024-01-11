![[Pasted image 20231004154320.png]]
> » Alayer is an isolated part of the application. * This can be a specific functionality offered in the application. Each layer should communicate with the layer above/below via well defined interfaces. + A layer will expose its functionality through an abstract API.

# Layers are losing popularity
---
![[Pasted image 20231004154459.png]]
> « Issues can arise in the development where the rules and principles of the layered pattern aren’t respected. May result in the Big Ball of Mud anti- pattern if it uses imports and functions instead of using abstraction via and API . « Lack of abstraction between layers, difficult to test and refactor/replace technology without effecting the entire system. + Potential single point of failure. » Monolithic application
