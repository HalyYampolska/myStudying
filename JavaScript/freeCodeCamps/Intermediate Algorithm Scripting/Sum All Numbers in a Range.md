# Introduction

We'll pass you an array of two numbers. Return the sum of those two numbers plus the sum of all the numbers between them. The lowest number will not always come first.

For example, sumAll([4,1]) should return 10 because sum of all the numbers between 1 and 4 (both inclusive) is 10.

## Before

```javascript
function sumAll(arr) {
  return 1;
}

sumAll([1, 4]);
```

## After

```javascript
function sumAll(arr) {
  let max = Math.max(arr[0], arr[1]);
  let min = Math.min(arr[0], arr[1]);
  let mySum = 0;
  for (let i = min; i <= max; i++) {
    mySum += i;
  }
  return mySum;
}

sumAll([1, 4]);
```
