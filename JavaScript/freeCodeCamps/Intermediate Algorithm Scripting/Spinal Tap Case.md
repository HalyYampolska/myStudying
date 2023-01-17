# Task 

Convert a string to spinal case. Spinal case is all-lowercase-words-joined-by-dashes.

## Before

```javascript
function spinalCase(str) {
  return str;
}

spinalCase('This Is Spinal Tap');
```

## After

```javascript
function spinalCase(str) {
  // Create a variable for the white space and underscores
  var regex = /\s+|_+/g;

  // Replace low-upper case to low-space-uppercase
  str = str.replace(/([a-z])([A-Z])/g, "$1 $2");

  // Replace space and underscore with
  return str.replace(regex, "-").toLowerCase();
}

spinalCase('This Is Spinal Tap');
```
