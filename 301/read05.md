
### 1- What is the single responsibility principle and how does it apply to components?

this principle means that every component should have one function to do, if the component has more 
than one function then make subcomponents as children to it, every child will do one function.

### 2- What does it mean to build a ‘static’ version of your application?

that is means you will not be able to change your data. in another meaning; you will not use state into your components.



### 3- Once you have a static application, what do you need to add?

you have to make it dynamic, by using states into each component that needs to change its data.

### 4- What are the three questions you can ask to determine if something is state?

if is it able to move from its component(parent to child)? if not, maybe it is not state.
if its value still fixed over time? if yes, it is not state.
if it depends on other states and props? if yes, it is not state.

### 5- How can you identify where state needs to live?

based on where it will be used and rendered? sometimes you have to pass this state from its component to another to render it there.
Things I want to know more about
classes in ES6.

# Higher-Order Functions

---


### 1-What is a “higher-order function”?

Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.
Higher-order functions allow us to abstract over actions, not just values. 

### 2-Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

compare between 2 values and return a boolean value


### 3-Explain how either map or reduce operates, with regards to higher-order functions

reduce >> It builds a value by repeatedly taking a single element from the array and combining it with the current value.

## Things I want to know more about

---

Higher-Order Functions