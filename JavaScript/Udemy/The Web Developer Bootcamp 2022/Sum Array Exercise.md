# Task 

Write a function called sumArray which accepts a single argument: an array of numbers.  It should return the sum of all the numbers in the array.

```javascript
sumArray([1,2,3]) // 6
sumArray([2,2,2,2]) // 8
sumArray([50,50,1]) // 101
```
## Hints

You'll need a variable to keep track of the total.  It should start out as zero.

Loop over the array and for each element, add it to the total variable.

After you have added every number to total, return total.

## Answer

```javascript
function sumArray(array) {
  for (var i = 0, sum = 0; i < array.length; sum += array[i++]);
  return sum;
}
```
