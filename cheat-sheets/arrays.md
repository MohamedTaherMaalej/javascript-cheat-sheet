# JavaScript Arrays Cheat Sheet

## Creating Arrays

```javascript
// Array literal
const fruits = ['apple', 'banana', 'orange'];

// Using the Array constructor
const numbers = new Array(1, 2, 3, 4, 5);
```

## Accessing Elements

```javascript
const fruits = ['apple', 'banana', 'orange'];

console.log(fruits[0]); // 'apple'
console.log(fruits.length); // 3
```

## Modifying Arrays

### Adding Elements

```javascript
const fruits = ['apple', 'banana', 'orange'];

// Add to the end
fruits.push('grape');

// Add to the beginning
fruits.unshift('kiwi');

// Add at a specific position
fruits.splice(2, 0, 'cherry');
```

### Removing Elements

```javascript
const fruits = ['apple', 'banana', 'orange'];

// Remove from the end
fruits.pop();

// Remove from the beginning
fruits.shift();

// Remove at a specific position
fruits.splice(1, 1);
```

### Updating Elements

```javascript
const fruits = ['apple', 'banana', 'orange'];

// Update an element
fruits[1] = 'pear';
```

## Iterating Through Arrays

### for Loop

```javascript
const fruits = ['apple', 'banana', 'orange'];

for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

### forEach Method

```javascript
const fruits = ['apple', 'banana', 'orange'];

fruits.forEach((fruit) => {
  console.log(fruit);
});
```

## Array Methods

### Map

```javascript
const numbers = [1, 2, 3, 4, 5];

const squaredNumbers = numbers.map((num) => num * num);
```

### Filter

```javascript
const numbers = [1, 2, 3, 4, 5];

const evenNumbers = numbers.filter((num) => num % 2 === 0);
```

### Reduce

```javascript
const numbers = [1, 2, 3, 4, 5];

const sum = numbers.reduce((acc, num) => acc + num, 0);
