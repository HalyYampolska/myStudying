# Task 

Find the smallest common multiple of the provided parameters that can be evenly divided by both, as well as by all sequential numbers in the range between these parameters.

The range will be an array of two numbers that will not necessarily be in numerical order.

For example, if given 1 and 3, find the smallest common multiple of both 1 and 3 that is also evenly divisible by all numbers between 1 and 3. The answer here would be 6.



## Before

```javascript
function smallestCommons(arr) {
  return arr;
}

smallestCommons([1,5]);
```

## After

```javascript
function smallestCommons(arr) {
  // Setup
  const [min, max] = arr.sort((a, b) => a - b);
  const numDivs = max - min + 1;
  // Largest possible value
  let upperBound = 1;
  for (let i = min; i <= max; i++) {
    upperBound *= i;
  }
  // All multiples of 'max'
  for (let multiple = max; multiple <= upperBound; multiple += max) {
  // Check every value 
  let divisorCount = 0;
  for (let i = min; i <= max; i++) {
    // Count divisors
  if (multiple % i === 0) {
    divisorCount +=1;
  }
  }
  if (divisorCount === numDivs) {
    return multiple;
  }
  }
  
}

smallestCommons([1,5]);
```
