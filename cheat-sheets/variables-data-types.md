# JavaScript Variables and Data Types Cheat Sheet

## Variables

### Declaration

```javascript
// Using var (not recommended in modern JavaScript)
var variableName = value;

// Using let (block-scoped variable)
let variableName = value;

// Using const (block-scoped constant)
const variableName = value;
```

### Variable Naming Rules

- Variable names are case-sensitive (`myVariable` and `myvariable` are different).
- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter, dollar sign, or underscore.
- Reserved words (e.g., `let`, `const`, `if`, `else`) cannot be used as variable names.

## Data Types

### Primitive Data Types

1. **Number:**
   ```javascript
   let num = 42;
   ```

2. **String:**
   ```javascript
   let greeting = 'Hello, World!';
   ```

3. **Boolean:**
   ```javascript
   let isTrue = true;
   ```

4. **Null:**
   ```javascript
   let myNull = null;
   ```

5. **Undefined:**
   ```javascript
   let undefinedVar;
   ```

6. **Symbol (ES6+):**
   ```javascript
   let sym = Symbol('unique');
   ```

### Composite Data Types

7. **Object:**
   ```javascript
   let person = {
     name: 'John Doe',
     age: 30,
     isStudent: false,
   };
   ```

8. **Array:**
   ```javascript
   let colors = ['red', 'green', 'blue'];
   ```

### Special Data Types

9. **Function:**
   ```javascript
   function greet(name) {
     return 'Hello, ' + name + '!';
   }
   ```

10. **Object (Date):**
    ```javascript
    let currentDate = new Date();
    ```

### Type Checking

```javascript
typeof variableName; // Returns a string representing the data type
```

### Type Conversion

- **To Number:**
  ```javascript
  let strNumber = '42';
  let num = Number(strNumber);
  ```

- **To String:**
  ```javascript
  let num = 42;
  let strNumber = String(num);
  ```

- **To Boolean:**
  ```javascript
  let truthyValue = 'Hello';
  let isTruthy = Boolean(truthyValue);
  ```

This cheat sheet provides a quick reference for declaring variables, naming rules, and different data types in JavaScript, including examples and basic type-checking and conversion techniques.
