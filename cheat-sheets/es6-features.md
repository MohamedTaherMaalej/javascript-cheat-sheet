# ES6 Features Cheat Sheet

## Let and Const

### Block-Scoped Declarations

```javascript
// Using let
let x = 10;

// Using const (constant)
const PI = 3.14;
```

## Arrow Functions

### Shorter Function Syntax

```javascript
// Traditional function expression
const add = function(a, b) {
  return a + b;
};

// Arrow function
const add = (a, b) => a + b;
```

## Template Literals

### String Interpolation

```javascript
const name = 'John';
const greeting = `Hello, ${name}!`;
```

## Destructuring Assignment

### Array Destructuring

```javascript
const numbers = [1, 2, 3];

const [a, b, c] = numbers;
```

### Object Destructuring

```javascript
const person = { name: 'Alice', age: 25 };

const { name, age } = person;
```

## Spread and Rest Operators

### Spread Operator

```javascript
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];

const combined = [...arr1, ...arr2];
```

### Rest Parameter

```javascript
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}

sum(1, 2, 3, 4); // 10
```

## Default Parameters

```javascript
function greet(name = 'Guest') {
  return `Hello, ${name}!`;
}
```

## Classes

### Class Definition

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    return `Hello, my name is ${this.name}.`;
  }
}

const person = new Person('John', 30);
```

## Promises

### Asynchronous Programming

```javascript
const fetchData = () => {
  return new Promise((resolve, reject) => {
    // asynchronous operation
    if (success) {
      resolve(data);
    } else {
      reject(error);
    }
  });
};
```

## Modules

### Exporting

```javascript
// module.js
export const PI = 3.14;
export function double(x) {
  return x * 2;
}

// main.js
import { PI, double } from './module';
