* We have to hide the sensitive data from the user by using the private keyword. 

* The user can access a variable using the methods get and set but now we can control the value. Example: A guy cannot be 8 metres.

*  It is easier to change one part of the code without affecting the others.

![[Pasted image 20230928112111.png]]
> Encapsulation Radius is a private public class Circle { member variable and can only be private int radius; fﬁzerfeetf‘;:r:ugh provided. public int getRadius() { return radius; } public void setRadius(int new_radius) { radius = new_radius; } }

![[Pasted image 20230928112130.png]]
> Encapsulation public class SomeClient { SomecClient (Circle circleA, Circle circleB){ These two lines of code will not be permitted — circleArradius=10; . |thesewillcausea circleB.radius = 12; compiler error circleA.setRadius(10); circleB.setRadius (12); Thisis how the radius attribute of Circle } objects must be accessed. }

![[Pasted image 20230928112210.png]]
> Encapsulat|0n Also, we can think of the . . . . circleA client object sending a message to each Circle object telling it to change its radius setRadius (10 Client Object setRadius (12) Some other object — the “client” circleB
