
# JavaScript Functions Cheat Sheet

## Function Declaration

```javascript
function functionName(parameters) {
  // code to be executed
  return result; // optional
}
```

## Function Expression

```javascript
const functionName = function(parameters) {
  // code to be executed
  return result; // optional
};
```

## Arrow Function (ES6+)

```javascript
const functionName = (parameters) => {
  // code to be executed
  return result; // optional
};
```

## Parameters and Arguments

```javascript
function addNumbers(a, b) {
  return a + b;
}

addNumbers(5, 3); // 8
```

## Default Parameters (ES6+)

```javascript
function greet(name = 'Guest') {
  return 'Hello, ' + name + '!';
}

greet(); // Hello, Guest!
greet('John'); // Hello, John!
```

## Rest Parameter (ES6+)

```javascript
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}

sum(1, 2, 3, 4); // 10
```

## Function Scope

```javascript
function example() {
  let localVar = 'I am a local variable';
  // localVar is only accessible within the function
}
```

## Closures

```javascript
function outerFunction() {
  let outerVar = 'I am from the outer function';

  function innerFunction() {
    console.log(outerVar); // inner function has access to outerVar
  }

  return innerFunction;
}

const closure = outerFunction();
closure(); // logs 'I am from the outer function'
```

## Callback Functions

```javascript
function fetchData(callback) {
  // asynchronous operation
  const data = fetchDataFromAPI();
  callback(data);
}

fetchData((result) => {
  console.log(result);
});
