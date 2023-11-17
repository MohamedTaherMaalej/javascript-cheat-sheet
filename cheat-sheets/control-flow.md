# JavaScript Control Flow Cheat Sheet

## Conditional Statements

### if Statement

```javascript
if (condition) {
  // code to be executed if the condition is true
} else {
  // code to be executed if the condition is false
}
```

### else if Statement

```javascript
if (condition1) {
  // code to be executed if condition1 is true
} else if (condition2) {
  // code to be executed if condition2 is true
} else {
  // code to be executed if no conditions are true
}
```

### switch Statement

```javascript
switch (expression) {
  case value1:
    // code to be executed if expression === value1
    break;
  case value2:
    // code to be executed if expression === value2
    break;
  // ... more cases ...
  default:
    // code to be executed if no cases match
}
```

## Loops

### for Loop

```javascript
for (let i = 0; i < 5; i++) {
  // code to be executed in each iteration
}
```

### while Loop

```javascript
let i = 0;
while (i < 5) {
  // code to be executed in each iteration
  i++;
}
```

### do-while Loop

```javascript
let i = 0;
do {
  // code to be executed in each iteration
  i++;
} while (i < 5);
```

## Jump Statements

### break Statement

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) {
    break; // exits the loop when i equals 5
  }
}
```

### continue Statement

```javascript
for (let i = 0; i < 5; i++) {
  if (i === 2) {
    continue; // skips the rest of the code block and continues with the next iteration
  }
  // code to be executed in each iteration, except when i equals 2
}
```

## Ternary Operator

```javascript
let result = (condition) ? 'true' : 'false';
// equivalent to:
// if (condition) {
//   result = 'true';
// } else {
//   result = 'false';
// }

