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

## Strings

```javascript
console.log("Deepesh" + " Sengar");
```

## Declaring variables

```javascript
let name = "Deepesh";
let number = 11;
console.log("Mr. " + name);
console.log(number + 4);
```

## Template Literals

Instead of '+' operator, we will use template literals

```javascript
const name = "Deepesh Sengar";
console.log(`Hello, My name is ${name}`);
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

## Arrays

```javascript
const fruits = ["apple", "banana", "orange"];
console.log(fruits);
console.log(fruits[0]);
console.log(fruits.length);
```

## Objects

Objects are used to group and manage multiple values
like key value pairs

```javascript
const item = { name: "Chocoloate", price: 30 };
console.log(item);
console.log(item.price);
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

```

```
