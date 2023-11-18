# JavaScript Objects Cheat Sheet

## Creating Objects

### Object Literal

```javascript
const person = {
  name: 'John Doe',
  age: 30,
  isStudent: false,
};
```

### Using the Object Constructor

```javascript
const car = new Object();
car.make = 'Toyota';
car.model = 'Camry';
car.year = 2022;
```

## Accessing Object Properties

```javascript
const person = {
  name: 'John Doe',
  age: 30,
  isStudent: false,
};

console.log(person.name); // 'John Doe'
console.log(person['age']); // 30
```

## Modifying Objects

```javascript
const person = {
  name: 'John Doe',
  age: 30,
  isStudent: false,
};

// Update a property
person.age = 31;

// Add a new property
person.city = 'New York';
```

## Deleting Object Properties

```javascript
const person = {
  name: 'John Doe',
  age: 30,
  isStudent: false,
};

delete person.age;
```

## Object Methods

```javascript
const person = {
  name: 'John Doe',
  age: 30,
  isStudent: false,
  greet: function() {
    console.log('Hello!');
  },
};

person.greet(); // 'Hello!'
```

## Object Iteration

```javascript
const person = {
  name: 'John Doe',
  age: 30,
  isStudent: false,
};

// Using for...in loop
for (let key in person) {
  console.log(key + ': ' + person[key]);
}
```

## Object Destructuring (ES6+)

```javascript
const person = {
  name: 'John Doe',
  age: 30,
  isStudent: false,
};

const { name, age } = person;
```

## Nested Objects

```javascript
const student = {
  name: 'Alice',
  age: 22,
  courses: {
    math: 'A',
    history: 'B',
  },
};
