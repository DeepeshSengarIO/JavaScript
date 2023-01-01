# Introduction

## Comments

```javascript
// Comment won`t be executed
```

## Calculations

```javascript
console.log(3);
console.log(5 + 2);
console.log(3 % 2);
```

## Data Types

Boolean
null
undefined
Number
BigInt
String
Symbol

## Strings

```javascript
console.log("Deepesh" + " Sengar");
```

## Declaring variables

var - Declare a variable, optionally init it to a value

```javascript
if (true) {
  var x = 5;
}
console.log(x); // x is 5
```

let - declare a block scoped, local variable, optionally initializing it to a value

const - declare a block scoped, read-only named constant

```javascript
if (Math.random() > 0.5) {
  const y = 5;
}
console.log(y); // ReferenceError: y is not defined
```

```javascript
let name = "Deepesh";
let number = 11;
console.log("Mr. " + name);
console.log(number + 4);
```

## + Operator

Instead of '+' operator, we will use template literals

```javascript
const name = "Deepesh Sengar";
console.log(`Hello, My name is ${name}`);
```

```javascript
x = "The answer is " + 42; // "The answer is 42"
y = 42 + " is the answer"; // "42 is the answer"
z = "37" + 7; // "377"
```

```javascript
"37" - 7; // 30
"37" * 7; // 259
```

## Type Casting

### parseInt()

a best practice for parseInt is to always include the radix parameter. The radix parameter is used to specify which numerical system is to be used.

```javascript
parseInt("101", 2); // 5
"1.1" +
  "1.1"(
    // '1.11.1'
    +"1.1"
  ) +
  +"1.1"; // 2.2
// Note: the parentheses are added for clarity, not required.
```

### parseFloat()

## Literals

Literals represent values in JavaScript. These are fixed values—not variables—that you literally provide in your script.

### Array Literals

```javascript
const coffees = ["French Roast", "Colombian", "Kona"];
const myList = ["home" /* empty */, , "school" /* empty */, ,];
```

### Object Literals

```javascript
const sales = "Toyota";

function carTypes(name) {
  return name === "Honda" ? name : `Sorry, we don't sell ${name}.`;
}

const car = { myCar: "Saturn", getCar: carTypes("Honda"), special: sales };

console.log(car.myCar); // Saturn
console.log(car.getCar); // Honda
console.log(car.special); // Toyota
```

```javascript
const car = { manyCars: { a: "Saab", b: "Jeep" }, 7: "Mazda" };

console.log(car.manyCars.b); // Jeep
console.log(car[7]); // Mazda
```

### Enhanced Object Literals

```javascript
const obj = {
  __proto__: theProtoObj,
  handler,
  toString() {
    return "d" + super.toString();
  },
  ["prop_" + (() => 42)]: 42,
};
```

### RegExp Literals

```javascript
const re = /ab+c/;
```

## Conditionals

```javascript
const number = 12;
if (number > 10) {
  console.log("Number is greater than 10");
}
```

## Boolean

```javascript
const number = 10;
console.log(number > 9);
```

## Comparison Operators

```javascript
const a = "2";
const b = 2;
console.log(a == b);
console.log(a === b);
console.log(a !== b);
```

## switch statement

```javascript
const color = "red";
switch (color) {
  case "red":
    console.log("stop");
    break;
  case "yellow":
    console.log("wait");
    break;
  default:
    console.log("go");
    break;
}
```

## While Loop

```javascript
let numbner = 1;
while (number < 100) {
  console.log(number);
  number++;
}
```

## For Loop

```javascript
for (let x = 1; x <= 10; x++) {
  console.log(x);
}
```

## Do - While

```javascript
let i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 5);
```

## Labled Statement

A label provides a statement with an identifier that lets you refer to it elsewhere in your program.

The Syntax

label:
statement

In this example, the label markLoop identifies a while loop.

```javascript
markLoop: while (theMark) {
  doSomething();
}
```

## Try - Catch

```javascript
openMyFile();
try {
  writeMyFile(theData); // This may throw an error
} catch (e) {
  handleError(e); // If an error occurred, handle it
} finally {
  closeMyFile(); // Always close the resource
}
```

## Arrays

```javascript
const fruits = ["apple", "banana", "orange"];
console.log(fruits);
console.log(fruits[0]);
console.log(fruits.length);
```

## For..of and For..in

for...in iterates over property names
for...of iterates over property values

```javascript
const arr = [3, 5, 7];
arr.foo = "hello";

for (const i in arr) {
  console.log(i);
}
// "0" "1" "2" "foo"

for (const i of arr) {
  console.log(i);
}
// Logs: 3 5 7
```

The for...of and for...in statements can also be used with destructuring.
For example, you can simultaneously loop over the keys and values of an object using Object.entries().

```javascript
const obj = { foo: 1, bar: 2 };

for (const [key, val] of Object.entries(obj)) {
  console.log(key, val);
}
// "foo" 1
// "bar" 2
```

## Objects

Objects are used to group and manage multiple values
like key value pairs

```javascript
const item = { name: "Chocoloate", price: 30 };
console.log(item);
console.log(item.price);
```

The following function takes as its argument an object and the object's name.

```javascript
function dumpProps(obj, objName) {
  let result = "";
  for (const i in obj) {
    result += `${objName}.${i} = ${obj[i]}<br>`;
  }
  result += "<hr>";
  return result;
}
```

## Objects as array elements

```javascript
const items = [
  { name: "Milk", price: "20" },
  { name: "Coffee", price: "15" },
];
console.log(items[0].name);
```

## Nested objects and Arrays

```javascript
const char = {
  name: "Deepesh Sengar",
  age: 20,
  favourite: {
    food: "Chicken Tikka Masala",
    sports: "Table Tennis",
    color: "Black",
  },
  langueges_known: ["Java", "JavaScript", "C++"],
};
```

## Functions

```javascript
const fun = function () {};
const fun = () => {};
const intro = (name, age) => {
  console.log(`I am ${name}`);
  console.log(`I am ${age} years old`);
};
intro("Deepesh Sengar", 22);
```

## Function Return Values

```javascript
const fun = () => {
  return 0;
};
```

## Objects and Functions

```javascript
const user = {
  name: "Deepesh Sengar",
  age: 22,
  greet: () => {
    console.log("Hello guys");
  },
};
user.greet();
```

## classes and constructors

```javascript
class animal{
    //constructor
    constructor(n, a){
        this.name = n,
        this.age = a,
    }
}
const animal  = new animal('Lion', 34);
```

## Methods

Functions that are belong to classes are called methods

```javascript
class Animal {
  constructor(name, age) {
    (this.age = age), (this.name = name);
  }
  greet() {
    console.log("Hello");
  }
}

const animal = new Animal("Lion", 35);
animal.greet();
```

## Inheritance

Create a new class based on the existing class

Animal Class ------Inherit--------> Dog Class

```javascript
class Animal{
    constructor(name, age){
        this.name = name,
        this.age = age,
    }
    info(){
        console.log(`Animal name is ${this.name}`);
        console.log(`Animal age is ${this.age}`);
    }
}

class Dog extends Animal{

}

const dog = new Dog('BullDog', 7);
dog.info();
```

## Return value in methods
