# Task

Remove all falsy values from an array. Return a new array; do not mutate the original array.

Falsy values in JavaScript are `false`, `null`, `0`, `""`, `undefined`, and `NaN`.

Hint: Try converting each value to a Boolean.

 ## Before

```javascript
function bouncer(arr) {
  return arr;
}

bouncer([7, "ate", "", false, 9]);
```

## After

### 1 

```javascript
function bouncer(arr) {
   const filteredArr = [];
  for (let i = 0; i < arr.length; i++) {
    if (arr[i]) filteredArr.push(arr[i]);
  }
  return filteredArr;
}

bouncer([7, "ate", "", false, 9]);
```

### 2 

```javascript
function bouncer(arr) {
   return arr.filter(Boolean);
}

bouncer([7, "ate", "", false, 9]);
```
