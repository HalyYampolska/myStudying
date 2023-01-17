# Task 

You will be provided with an initial array (the first argument in the destroyer function), followed by one or more arguments. Remove all elements from the initial array that are of the same value as these arguments.

Note: You have to use the arguments `object`.

## Before

```javascript
function destroyer(arr) {
  return arr;
}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);
```

## After

```javascript
function destroyer(arr) {
  const removeNum = Object.values(arguments).slice(1);
  const filteredArray = [];

  for (let i = 0; i < arr.length; i++) {
    let removeElement = false;
    for (let j = 0; j < removeNum.length; j++) {
      if (arr[i] === removeNum[j]) {
        removeElement = true;
      }
    }
    if (!removeElement) {
      filteredArray.push(arr[i]);
    }
  }
  return filteredArray;

}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);
```
