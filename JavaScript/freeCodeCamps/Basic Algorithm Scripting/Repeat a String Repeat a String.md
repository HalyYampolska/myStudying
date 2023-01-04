# Task

Repeat a given string `str` (first argument) for `num` times (second argument). Return an empty string if `num` is not a positive number. For the purpose of this challenge, do not use the built-in `.repeat()` method.

 ## Before

```javascript
function repeatStringNumTimes(str, num) {
  return str;
}

repeatStringNumTimes("abc", 3);
```

## After

```javascript
function repeatStringNumTimes(str, num) {
    if(num <= 0) 
      return "";
    if(num === 1) 
      return str;
    else 
      return str + repeatStringNumTimes(str, num - 1);
}

repeatStringNumTimes("abc", 3);
```
