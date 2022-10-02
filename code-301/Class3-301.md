# lists and keys
* What does .map() return? 
**return a new array that has the same length of previous array**
* If I want to loop through an array and display each value in JSX, how do I do that in React? 

**You can build collections of elements and include them in JSX using curly braces {}, by using map.**
 * Each list item needs a unique **key**.
* What is the purpose of a key?
> Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity(1)


 # The Spread Operator
 * What is the spread operator?
 **the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.**

* List 4 things that the spread operator can do.

1. Copying an array
2. Concatenating or combining arrays
3. Using Math functions
4. Using an array as arguments
* Give an example of using the spread operator to combine two arrays.
* Give an example of using the spread operator to add a new item to an array.
> const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩(2)

* Give an example of using the spread operator to combine two objects into one.

> const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂 (3)


# How to Pass Functions Between Components

In the video, what is the first step that the developer does to pass functions between components?
**create it when you want to change state, by create variable and equal to this.state.array**

In your own words, what does the increment function do?
**increase by one the value of specfic key**



How can you pass a method from a parent component into a child component?
**variable={this.method}**

How does the child component invoke a method that was passed to it from a parent component?
**this.props.method**

## Things I want to know more about

1. cited by [list and key doc](https://reactjs.org/docs/lists-and-keys.html)
2. cited by[spread operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
3. cited by[spread operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

