2023-09-22

* Lecturer email: pierpaolo.dondio@tudublin.ie

* [[Paradigm Definition]]

* **Procedural:** Logic where the flow (I.E the movement through the code) is also defined by the logic

* In Logical and Functional programming, you do not define the flow. 

* Factorial code example:
```python   
def factorial(count: int, total: int) -> int:
	'''Takes the number to be factorised then returns the factorised number, total should ALWAYS be 1'''
    if count == 0:
        return total
    else:
        return factorial(count-1, total*count)

input = int(input("Enter a number: "))
print(factorial(input, 1))
```

* A loop is generally more memory efficient then a recursive loop as the memory can be freed as the logic progresses, not only when finished. 

* 