# Task 

Return the number (count) of vowels in the given string.

We will consider `a`, `e`, `i`, `o`, `u` as vowels for this Kata (but not `y`).

The input string will only consist of lower case letters and/or spaces.

## Solution with logic (comments)

```
<?php
function getCount($str) {
  // Perform a global regular expression match
  $vowelsCount = preg_match_all('/[aeiou]/',$str);
  return $vowelsCount;
}
?>
```
