# Task 

Let's get some practice using the filter method. Write a function called `validUserNames` that accepts an array of `usernames` (strings).  It should return a new array, containing only the usernames that are less than 10 characters. For example:

```javascript
validUserNames(['mark', 'staceysmom1978', 'q29832128238983', 'carrie98', 'MoanaFan']);
```

Note: The syntax for this solution might be a little strange to you at this point in the course because it requires you to write the code, that you just learned in the previous lecture, inside of a function. e.g.,

## Answer

```javascript
function validUserNames(usernames) {
  return usernames.filter(function(usernames) {
  return usernames.length < 10;     
  })  
}
```


