# Introduction

The `every` method works with arrays to check if every element passes a particular test. It returns a Boolean value - `true` if all values meet the criteria, `false` if not.

For example, the following code would check if every element in the `numbers` array is less than 10:
```javascript
const numbers = [1, 5, 8, 0, 10, 11];

numbers.every(function(currentValue) {
  return currentValue < 10;
});
```
The `every` method would return `false` here.

## Task 

Use the `every` method inside the `heckPositive` function to check if every element in arr is positive. The function should return a Boolean value.

## Before

```javascript
function checkPositive(arr) {
  // Only change code below this line


  // Only change code above this line
}

checkPositive([1, 2, 3, -4, 5]);
```

## After

```javascript
function checkPositive(arr) {
  // Only change code below this line
  return arr.every(function(num) { 
  return num > 0;   
});
  // Only change code above this line
}

checkPositive([1, 2, 3, -4, 5]);
```
