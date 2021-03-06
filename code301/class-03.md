[Home Page](https://devaoc.github.io/reading-notes/)

# Class 03 Notes

## React Docs - Lists and Keys

The map function returns an array. It can be an array of anything that was contained in the previous array that you used map on.

All you must do to display elements in JSX is to add {} around the variable containing the information.

Each list item needs a unique key. The purpose of such a key is to give the react element a stable identity.

## The Spread Operator

The spread operator is ..., it is used to expands iterable objects into lists of arguements.

For example:

```Javascript

Math.max(1,3,5) // 5
Math.max([1,3,5]) // NaN
Math.max(...[1,3,5]) // 5

```

It can also be used for:

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Adding an item to a list
- Adding a state in React
- Combining objects
- Converting NodeList to an array

Example of combining arrays:

```Javascript

const myArray = [`ðĪŠ`,`ðŧ`,`ð`]
const yourArray = [`ð`,`ðĪ`,`ðĪĐ`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // ðĪŠ ðŧ ð ð ðĪ ðĪĐ

```

Example of adding new items to an array:

```Javascript

const fewFruit = ['ð','ð','ð']
const fewMoreFruit = ['ð', 'ð', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "ð", "ð", "ð", "ð", "ð" ]

```

Example of combining objects:

```Javascript

const objectOne = {hello: "ðĪŠ"}
const objectTwo = {world: "ðŧ"}
const objectThree = {...objectOne, ...objectTwo, laugh: "ð"}
console.log(objectThree) // Object { hello: "ðĪŠ", world: "ðŧ", laugh: "ð" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("ð".repeat(5))}}
objectFour.laugh() // ððððð

```

## How to Pass Funcitons Between Components

## Things I want to know more about
