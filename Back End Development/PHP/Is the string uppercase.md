# Task 

Create a method to see whether the string is ALL CAPS.

Examples (input -> output)

1. "c" -> False
2. "C" -> True
3. "hello I AM DONALD" -> False
4. "HELLO I AM DONALD" -> True
5. "ACSKLDFJSgSKLDFJSKLDFJ" -> False
6. "ACSKLDFJSGSKLDFJSKLDFJ" -> True

A string is said to be in ALL CAPS whenever it does not contain any lowercase letter so any string containing no letters at all is trivially considered to be in ALL CAPS.

## Solution with logic (comments)

```
<?php
// Accepts a string
function is_uppercase($str) {
  // Looping through all characters in a string
  for ($i = 0; $i < strlen($str); $i++) {
    // Checking whether a character in a string is lowercase or uppercase
    if (ctype_lower($str[$i])) {
      // If at least one element in the term is lowercase, we return a false
      return false;
    }
  }
  return true;
}
?>
```
