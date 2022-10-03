# Intro to Python
---
>## Big O :
### - What is Big O  ?
<font size="2"> Big O notation is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity.</font> 

---
## Types And Values in Python

As in many programming languages, a Python assignment statement associates a symbolic name on the left-hand side with a value on the right-hand side. In Python, we say that names refer to values, or a name is a reference to a value

Python keeps track of how many references each value has, and automatically cleans up values that have none. This is called “garbage collection,” and means that you don’t have to get rid of values, they go away by themselves when they are no longer needed.

---
##  Facts and Myths about Python names and values :

 Since everything in Python is an object, we should reiterate that assigning a variable to another variable does not actually copy the value's content; rather, it copies the reference to the value or memory location that the other variable refers to in memory. Reassigning a different value to a variable again does not mean that we just replaced the original value; rather, it means that we actually broke the first link or reference and added a new one to a different memory location. In conclusion, assignment does not copy data, whichAdditionally, this indicates that operations take place not on the variables themselves but rather on data or values.
 When a variable has a value of an immutable type, changing that value or performing operations on it, such as adding to it or assigning a new value, breaks the reference and creates a new one for the new value because we cannot change the value in place.
While changing an immutable type results in rebinding, we can rebind mutable types in some ways, such as by adding to a list, so change and mutation are not always synonymous.The assignment, on the other hand, is the same for both types.
A lot of things, like defining a class or assigning the iterator in a for loop, are assignments, and assigning is not just limited to the equal sign "=."
Because local variables are destroyed after a job is finished, we should exercise caution when passing arguments to functions or local scopes, such as by reference and value.Even if the values passed are mutable, we should always try to avoid generating side effects by copying them, especially if they are.
Names are not restricted to particular types of values; they can be reassigned dynamically without difficulty, and a variable can reference a regular number and then a function without difficulty.
Moreover, despite the fact that the subject of the video appears to be straightforward, I believe it to be of crucial importance.

---
>### Sources : 
https://www.freecodecamp.org/news/big-o-notation-why-it-matters-and-why-it-doesnt-1674cfa8a23c/

https://www.codenewbie.org/basecs/8

https://www.youtube.com/watch?v=_AEJHKGk9ns&ab_channel=PyCon2015