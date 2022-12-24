# Introduction

You've learned shortcuts for common string patterns like alphanumerics. Another common pattern is looking for just digits or numbers.

The shortcut to look for digit characters is `\d`, with a lowercase d. This is equal to the character class `[0-9]`, which looks for a single character of any number between zero and nine.

## Task 
Use the shorthand character class `\d` to count how many digits are in movie titles. Written out numbers ("six" instead of 6) do not count.

## Before

```javascript
let movieName = "2001: A Space Odyssey";
let numRegex = /change/; // Change this line
let result = movieName.match(numRegex).length;
```

## After

```javascript
let movieName = "2001: A Space Odyssey";
let numRegex = /\d/ig; // Change this line
let result = movieName.match(numRegex).length;
```
