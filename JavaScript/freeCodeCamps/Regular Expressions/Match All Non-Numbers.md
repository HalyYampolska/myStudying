# Introduction

The last challenge showed how to search for digits using the shortcut `\d` with a lowercase `d`. You can also search for non-digits using a similar shortcut that uses an uppercase `D` instead.

The shortcut to look for non-digit characters is `\D`. This is equal to the character class `[^0-9]`, which looks for a single character that is not a number between zero and nine.

## Task 
Use the shorthand character class for non-digits `\D` to count how many non-digits are in movie titles.

## Before

```javascript
let movieName = "2001: A Space Odyssey";
let noNumRegex = /change/; // Change this line
let result = movieName.match(noNumRegex).length;
```

## After

```javascript
let movieName = "2001: A Space Odyssey";
let noNumRegex = /\D/ig; // Change this line
let result = movieName.match(noNumRegex).length;
```
