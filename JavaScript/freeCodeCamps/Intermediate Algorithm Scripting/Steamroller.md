# Task 

Flatten a nested array. You must account for varying levels of nesting.

## Before

```javascript
function steamrollArray(arr) {
  return arr;
}

steamrollArray([1, [2], [3, [[4]]]]);
```

## After

```javascript
function steamrollArray(arr) {
  const flatArr = [];
  for (let i = 0; i < arr.length; i++) {
    if (Array.isArray(arr[i])) {
      arr.push(...steamrollArray(arr[i]));
    } else {
      flatArr.push(arr[i]);
    }
  }
  return flatArr;
}

steamrollArray([1, [2], [3, [[4]]]]);
```
