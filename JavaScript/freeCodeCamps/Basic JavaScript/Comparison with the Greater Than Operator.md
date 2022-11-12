# Introduction

The greater than operator (`>`) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns `true`. Otherwise, it returns `false`.

Like the equality operator, the greater than operator will convert data types of values while comparing.

## Exemples

```javascript
5   >  3  // true
7   > '3' // true
2   >  3  // false
'1' >  9  // false
```

## Task

Add the greater than operator to the indicated lines so that the return statements make sense.

```javascript
function welcomeToBooleans() {
  // Only change code below this line
  return true; // Change this line
  // Only change code above this line
}
```

## Before

```javascript
function testGreaterThan(val) {
  if (val) {  // Change this line
    return "Over 100";
  }

  if (val) {  // Change this line
    return "Over 10";
  }

  return "10 or Under";
}

testGreaterThan(10);
```

## After

```javascript
function testGreaterThan(val) {
  if (val > 100) {  // Change this line
    return "Over 100";
  }

  if (val > 10) {  // Change this line
    return "Over 10";
  }

  return "10 or Under";
}

testGreaterThan(10);
```
