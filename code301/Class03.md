# Passing Functions as Props

## React Docs - lists and keys
1. What does .map() return?

    It's return a new array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

    We can use map() function to lopp through an array and return its values as JSX element using curly braces {} and thethem inside an array.

3. Each list item needs a unique key .

4. What is the purpose of a key?

    Keys help React identify which items have changed, are added, or are removed.

## The Spread Operator
1. What is the spread operator?

    Is a syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

2. List 4 things that the spread operator can do.
    * Copying an array
    * Concatenating or combining arrays
    * Using Math functions
    * Using an array as arguments

3. Give an example of using the spread operator to combine two arrays.
```
let firstArray = ['A','B','C']
let secondArray = ['D','E','F']
let newrArray = [...firstArray,...secondArray]
console.log(...newrArray) // A B C D E F
```
4. Give an example of using the spread operator to add a new item to an array.
```
let firstArray = ['A','B','C']
let secondArray = ['D','E', ...firstArray]
console.log(secondArray) //  Array(5) [ "D", "E", "A", "B", "C" ]
```
5. Give an example of using the spread operator to combine two objects into one
```
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
```

## How to Pass Functions Between Components
1. In the video, what is the first step that the developer does to pass functions between components?

    He create a functions where to state going to change

2. In your own words, what does the increment function do?

    It finding the match object in order to change it state.

3. How can you pass a method from a parent component into a child component?

    We can pass a method by using props.

4. How does the child component invoke a method that was passed to it from a parent component?