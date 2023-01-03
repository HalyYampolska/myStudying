# Task

Reverse the provided string and return the reversed string.

For example, `"hello"` should become `"olleh"`.

 ## Before

```javascript
function reverseString(str) {
  return str;
}

reverseString("hello");
```

## After

```javascript
function reverseString(str) {
  return str.split("").reverse().join("");
}

reverseString("hello");
```
