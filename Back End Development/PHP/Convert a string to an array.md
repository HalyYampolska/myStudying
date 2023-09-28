# Task 

Write a function to split a string and convert it into an array of words.

Examples (Input ==> Output):
```
"Robin Singh" ==> ["Robin", "Singh"]

"I love arrays they are my favorite" ==> ["I", "love", "arrays", "they", "are", "my", "favorite"]
```

## Solution with logic (comments)

```
<?php
function string_to_array($s){
  // Use explode to split the string into an array of words
  return explode(' ', $s);
}
?>
```
