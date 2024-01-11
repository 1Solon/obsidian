**General Notes:**
* JavaScript is always passed by value, but for objects that value of the variable is a reference.

* Because of this, when you pass an object and change its properties, those changes persist outside of the function.

* This makes it look like it’s pass by reference

* But if you actually change the value of the object variable, you will see that the change does not persist, proving it's really pass by value.

**Example:**
![[Pasted image 20210928122504.png]]

**Output:**
![[Pasted image 20210928122527.png]]