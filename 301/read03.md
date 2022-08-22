# Map function and Spread Operator

*This class talks about how to use the map function and the spread operator*

## Map()
1. What does .map() return?
- It returns a new array as a result of the callback function.

2. If I want to loop through an array and display each value in JSX, how do I do that in React?
- Using the map function to loop through the array and use {curly brackets} of the elements.

3. Each list item needs a unique ____.
- Key

4. What is the purpose of a key?
- Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.


## The Spread Operator

1. What is the spread operator?
- The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.


2. List 4 things that the spread operator can do.
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list

3. Give an example of using the spread operator to combine two arrays.
- const array1 = [1,2,3]
const array2 = [4,5,6]
const combinedArray = [...array1,...array2]
combinedArray = [1,2,3,4,5,6]

4. Give an example of using the spread operator to add a new item to an array.
- const item = [1]
const array = [1,2,3,...item]

5. Give an example of using the spread operator to combine two objects into one.

- const object1 = {fname: "Mohannad"}
const object2 = {lname: ghbashneh}
const combinedObject = {...object1,...object2}
combinedObject = {fname: "Mohannad", lname: ghbashneh}

## Passing Functions between components

1. In the video, what is the first step that the developer does to pass functions between components?
- Creating the functions with the state

2. In your own words, what does the increment function do?
- Used to loop through the objects and if the name matches the one in the function it increments one to loop to the next name

3. How can you pass a method from a parent component into a child component?
- Using {this.iten}

4. How does the child component invoke a method that was passed to it from a parent component?
- By using the property to call the function

