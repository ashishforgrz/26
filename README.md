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

JavaScript Sets - 
// Create a Set
const letters = new Set();

// Add some values to the Set
letters.add("a");
letters.add("b");
letters.add("c");

JavaScript Classes -
JavaScript Classes are templates for JavaScript Objects
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}

JavaScript Promises -
Object that links `Producing Code` and `Consuming Code`
const myPromise = new Promise(function(myResolve, myReject) {
  setTimeout(function() { myResolve("I love You !!"); }, 3000);
});

myPromise.then(function(value) {
  document.getElementById("demo").innerHTML = value;
});

The Symbol Type - 
 represents a unique `hidden` identifier that no other code can accidentally access
 
Default Parameter Values -
ES6 allows function parameters to have default values
function myFunction(x, y = 10) {
  // y is 10 if not passed or undefined
  return x + y;
}
myFunction(5); // will return 15

Function Rest Parameter -
allows a function to treat an indefinite number of arguments as an array
function sum(...args) {
  let sum = 0;
  for (let arg of args) sum += arg;
  return sum;
}

let x = sum(4, 9, 16, 25, 29, 100, 66, 77);

