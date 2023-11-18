# JavaScript Promises Cheat Sheet

## Creating a Promise

```javascript
const myPromise = new Promise((resolve, reject) => {
  // Async operation or logic here
  if (success) {
    resolve(result);
  } else {
    reject(error);
  }
});
```

## Handling Promise States

### Resolved (Fulfilled)

```javascript
myPromise.then((result) => {
  // Handle the resolved state
  console.log(result);
});
```

### Rejected

```javascript
myPromise.catch((error) => {
  // Handle the rejected state
  console.error(error);
});
```

### Finally (ES2018+)

```javascript
myPromise.finally(() => {
  // Code to be executed regardless of the promise state
});
```

## Chaining Promises

```javascript
myPromise
  .then((result) => {
    // First callback
    return modifyResult(result);
  })
  .then((modifiedResult) => {
    // Second callback
    console.log(modifiedResult);
  })
  .catch((error) => {
    // Handle any errors in the chain
    console.error(error);
  });
```

## Promise.all

```javascript
const promise1 = fetchDataFromAPI();
const promise2 = fetchAnotherData();

Promise.all([promise1, promise2])
  .then(([result1, result2]) => {
    // Handle both results
    console.log(result1, result2);
  })
  .catch((error) => {
    // Handle any errors in the promises
    console.error(error);
  });
```

## Promise.race

```javascript
const promise1 = fetchDataFromAPI();
const promise2 = fetchAnotherData();

Promise.race([promise1, promise2])
  .then((firstResult) => {
    // Handle the result of the first resolved promise
    console.log(firstResult);
  })
  .catch((error) => {
    // Handle any errors in the promises
    console.error(error);
  });
