# Task 

Find the missing letter in the passed letter range and return it.

If all letters are present in the range, return `undefined`.

## Before

```javascript
function fearNotLetter(str) {
  return str;
}

fearNotLetter("abce");
```

## After

```javascript
function fearNotLetter(str) {
  for (let i = 1; i < str.length; ++i) {
    if (str.charCodeAt(i) - str.charCodeAt(i - 1) > 1) {
      return String.fromCharCode(str.charCodeAt(i - 1) + 1);
    }
  }
}

fearNotLetter("abce");
```
