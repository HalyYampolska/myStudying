# Introduction

If you have multiple conditions that need to be addressed, you can chain `if` statements together with `else if` statements.

## Exemple 

```javascript
if (num > 15) {
  return "Bigger than 15";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 15";
}
```

## Task 
Convert the logic to use `else if` statements.

## Before

```javascript
function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }

  if (val < 5) {
    return "Smaller than 5";
  }

  return "Between 5 and 10";
}

testElseIf(7);
```

## After

```javascript
function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  } else if (val < 5) {
    return "Smaller than 5";
  } else {
    return "Between 5 and 10";
}

testElseIf(7);
}
```
