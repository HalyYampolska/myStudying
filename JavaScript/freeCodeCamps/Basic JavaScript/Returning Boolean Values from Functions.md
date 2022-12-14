# Introduction

You may recall from Comparison with the Equality Operator that all comparison operators return a boolean `true` or `false` value.

Sometimes people use an `if`/`else` statement to do a comparison, like this:

```javascript
function isEqual(a, b) {
  if (a === b) {
    return true;
  } else {
    return false;
  }
}
```

But there's a better way to do this. Since `===` returns `true` or `false`, we can return the result of the comparison:

```javascript
function isEqual(a, b) {
  return a === b;
}
```

## Task 
Fix the function isLess to remove the `if`/`else` statements.

## Before

```javascript
function isLess(a, b) {
  // Only change code below this line
  if (a < b) {
    return true;
  } else {
    return false;
  }
  // Only change code above this line
}

isLess(10, 15);
```

## After

```javascript
function isLess(a, b) {
  // Only change code below this line
    return a < b;
  // Only change code above this line
}

isLess(10, 15);
```
