# Task 

Given a positive integer `num`, return the sum of all odd Fibonacci numbers that are less than or equal to `num`.

The first two numbers in the Fibonacci sequence are 1 and 1. Every additional number in the sequence is the sum of the two previous numbers. The first six numbers of the Fibonacci sequence are 1, 1, 2, 3, 5 and 8.

For example, `sumFibs(10)` should return `10` because all odd Fibonacci numbers less than or equal to `10` are 1, 1, 3, and 5.

## Before

```javascript
function sumFibs(num) {
  return num;
}

sumFibs(4);
```

## After

```javascript
function sumFibs(num) {
  let firstNum = 0;
  let nextNum = 1;
  let result  = 0;
  while (nextNum <= num) {
    if (nextNum % 2 !== 0) {
      result += nextNum;
    }
    nextNum += firstNum;
    firstNum = nextNum - firstNum; 
  }
  return result;
}

sumFibs(4);
```
