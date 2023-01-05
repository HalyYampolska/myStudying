# Task

Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.

For the purpose of this exercise, you should also capitalize connecting words like `the` and `of`.

 ## Before

```javascript
function titleCase(str) {
  return str;
}

titleCase("I'm a little tea pot");
```

## After

### 1
```javascript
function titleCase(str) {
   str = str.toLowerCase().split(' ');
  for (var i = 0; i < str.length; i++) {
    str[i] = str[i].charAt(0).toUpperCase() + str[i].slice(1); 
  }
  return str.join(' ');
}

titleCase("I'm a little tea pot");
```

### 2
```javascript
function titleCase(str) {
   return str.toLowerCase().split(' ').map(function(word) {
    return (word.charAt(0).toUpperCase() + word.slice(1));
  }).join(' ');
}

titleCase("I'm a little tea pot");
```
