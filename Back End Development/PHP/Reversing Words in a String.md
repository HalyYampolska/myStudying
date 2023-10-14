# Task 

You need to write a function that reverses the words in a given string. A word can also fit an empty string. If this is not clear enough, here are some examples:

As the input may have trailing spaces, you will also need to ignore unneccesary whitespace.

Example (Input --> Output)
```
"Hello World" --> "World Hello"
"Hi There." --> "There. Hi"
```

## Solution with logic (comments)

```
<?php
function reverse($string) {
  return implode(" ", array_reverse(explode(" ", $string))); // explode(" ", $string) - create massiv with a gap, array_reverse - reverse part of massive, implode - create a string with the gap 
}
?>
```
