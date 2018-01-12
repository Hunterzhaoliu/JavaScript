# JavaScript
Learning to build and design website

## General Notes

syntax with semicolon on ends of lines

### Introduction

console.log() prints material
"" or '' creates a string
4 data types:
1. String
2. Number
3. Boolean
4. Null
5. undefined

### Built-in Methods

[List of JavaScript Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/prototype)
[List of Math Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)
[List of Number Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)
```javascript
.length 
.toUpperCase()
.startsWith(letter) #produces boolean
// single line comment
/*
multiline comment
*/
const var_name = ; //const stands for constant and creates a variable with a value that cannot change
//camelCasing is when each new word begins with a capitalized letter
let var_name = ;
var_name = ;
//let var allows for the value that var_name has to be changed
//if a let var is not set to a value, it becomes undefined
let var_name;
console.log(var_name);
//string interpolation allows to print variables
const favoriteAnimal = 'human';
console.log('My favorite animal' + favoriteAnimal);
//another form of string interpolation known as ES6
const myName = 'Hunter';
const myCity = 'NYC';
console.log(`My name is ${myName}. My favorite city is ${myCity}.`);
+=
-=
*=
++
--
=== //equavilent
! //changes truthy to falsy 
<
>
<=
>=
!==
&&
||
```

### Control Flow

```javascript
if (condition_name) {
  block
} else {
  block
}

//can use a variable condition that has a string bc every variable has a truthy or falsy value
let variableOne = 'I Exist!';
if (variableOne) {
// This code will run because variableOne contains a truthy value.
} else {
// This code will not run because the first block ran.
}

switch //like an if/else statement without all of the syntax
let groceryItem = 'papaya';

switch (groceryItem) {
  case 'tomato':
    console.log('Tomatoes are $0.49');
    break;
  case 'lime':
    console.log('Limes are $1.49');
    break;
  case 'papaya':
    console.log('Papayas are $1.29');
    break;
  default:
    console.log('Invalid item');
    break;
}

//Ternary operator is another replacement for if/else

isNightTime ? 
console.log('Turn on the lights!') : 
console.log('Turn off the lights!');
```
### Functions

```javascript
//Function expression is used to declare a function
() => //arrow function syntax that indicates a variable will store a function
let calculatorIsOn = false;

const pressPowerButton = () => { //put parameters in ()
  if (calculatorIsOn) {
    console.log('Calculator turning off.');
    calculatorIsOn = false;
  } else {
    console.log('Calculator turning on.');
    calculatorIsOn = true;
  }
};

pressPowerButton();
// Output: Calculator turning on.

pressPowerButton();
// Output: Calculator turning off.

//function declaration can also create a function just with different syntax
function square (number) {
  return number * number; 
}

console.log(square(5));
// Output: 25.
```

### Loops

`for` loop syntax:

```javascript
for (init_value; max_value; incrementation_value) {
}
```

### Data Structures

`let array_name = [thing_one, thing_two, thing_n]; //creates an array with thing_one through thing_n;`
`array_name[index] = new_value;`
`.push()` adds items to the end of an array
`.pop()` removes the last item of an array
`.shift()` removes the first item of an array
`.unshift()` adds element(s) to the beginning of an array
`.slice(init_index, final_index)` creates a new array with the items from in between the index
[Method Library](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
