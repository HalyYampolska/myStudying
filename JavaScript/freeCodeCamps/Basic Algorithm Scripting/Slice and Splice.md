# Task

You are given two arrays and an index.

Copy each element of the first array into the second array, in order.

Begin inserting elements at index `n` of the second array.

Return the resulting array. The input arrays should remain the same after the function runs.

 ## Before

```javascript
function frankenSplice(arr1, arr2, n) {
  return combinedArrays
}

frankenSplice([1, 2, 3], [4, 5, 6], 1);
```

## After

```javascript
function frankenSplice(arr1, arr2, n) {
  let combinedArrays = arr2.slice()
  combinedArrays.splice(n, 0, ...arr1)
  return combinedArrays
}

frankenSplice([1, 2, 3], [4, 5, 6], 1);
```
