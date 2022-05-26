# 26/05/2022
 
=>>ES6 -
second major revision to JavaScript

JavaScript let -
The let keyword allows you to declare a variable with block scope
var x = 10;
// Here x is 10
{
  let x = 2;
  // Here x is 2
}
// Here x is 10

JavaScript const -
The const keyword allows you to declare a constant
var x = 10;
// Here x is 10
{
  const x = 2;
  // Here x is 2
}
// Here x is 10

Arrow Functions
Arrow functions allows a short syntax for writing function expressions
// ES5
var x = function(x, y) {
   return x * y;
}

// ES6
const x = (x, y) => x * y;

The For/Of Loop -
The JavaScript for/of statement loops through the values of an iterable objects

Looping over an Array -
const cars = ["BMW", "Volvo", "Mini"];
let text = "";

for (let x of cars) {
  text += x + " ";
}

Looping over a String -
let language = "JavaScript";
let text = "";

for (let x of language) {
    text += x + " ";
}

JavaScript Maps -
// Create Objects
const apples = {name: 'Apples'};
const bananas = {name: 'Bananas'};
const oranges = {name: 'Oranges'};

// Create a new Map
const fruits = new Map();

// Add new Elements to the Map
fruits.set(apples, 500);
fruits.set(bananas, 300);
fruits.set(oranges, 200);


