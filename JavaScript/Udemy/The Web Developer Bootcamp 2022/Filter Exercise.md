# Task 

Let's get some practice using the filter method. Write a function called `validUserNames` that accepts an array of `usernames` (strings).  It should return a new array, containing only the usernames that are less than 10 characters. For example:

```javascript
validUserNames(['mark', 'staceysmom1978', 'q29832128238983', 'carrie98', 'MoanaFan']);
```

## Answer

```javascript
function validUserNames(usernames) {
  return usernames.filter(function(usernames) {
  return usernames.length < 10;     
  })  
}
```
