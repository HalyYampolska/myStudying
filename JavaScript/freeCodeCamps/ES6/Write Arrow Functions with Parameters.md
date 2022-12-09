# Introduction
Just like a regular function, you can pass arguments into an arrow function.
```javascript
const doubler = (item) => item * 2;
doubler(4);
```
`doubler(4)` would return the value `8`.

If an arrow function has a single parameter, the parentheses enclosing the parameter may be omitted.

```javascript
const doubler = item => item * 2;
```

It is possible to pass more than one argument into an arrow function.

```javascript
const multiplier = (item, multi) => item * multi;
multiplier(4, 2);
```
`multiplier(4, 2)` would return the value `8`.

## Task 
Rewrite the `myConcat` function which appends contents of `arr2` to `arr1` so that the function uses arrow function syntax.

## Before

```javascript
var myConcat = function(arr1, arr2) {
  return arr1.concat(arr2);
};

console.log(myConcat([1, 2], [3, 4, 5]));
```

## After

```javascript
const myConcat = (arr1, arr2) => arr1.concat(arr2)

myConcat([1, 2], [3, 4, 5])
```
