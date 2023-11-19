# JavaScript Async/Await Cheat Sheet

## Async Function Declaration

```javascript
async function myAsyncFunction() {
  // Asynchronous code here
  return result;
}
```

## Await Keyword

```javascript
async function fetchData() {
  const result = await fetch('https://api.example.com/data');
  const data = await result.json();
  return data;
}
```

## Handling Errors

```javascript
async function fetchData() {
  try {
    const result = await fetch('https://api.example.com/data');
    const data = await result.json();
    return data;
  } catch (error) {
    // Handle errors here
    console.error(error);
  }
}
```

## Async/Await with Promise.all

```javascript
async function fetchData() {
  try {
    const [data1, data2] = await Promise.all([
      fetch('https://api.example.com/data1'),
      fetch('https://api.example.com/data2'),
    ]);

    const parsedData1 = await data1.json();
    const parsedData2 = await data2.json();

    return { data1: parsedData1, data2: parsedData2 };
  } catch (error) {
    console.error(error);
  }
}
```

## Using Async/Await in a Function

```javascript
const processData = async () => {
  try {
    const result = await fetchData();
    console.log(result);
  } catch (error) {
    console.error(error);
  }
};

processData();
```

## Async/Await with Promises

```javascript
const fetchData = () => {
  return new Promise((resolve, reject) => {
    // Asynchronous operation
    if (success) {
      resolve(data);
    } else {
      reject(error);
    }
  });
};

const processData = async () => {
  try {
    const result = await fetchData();
    console.log(result);
  } catch (error) {
    console.error(error);
  }
};

processData();
