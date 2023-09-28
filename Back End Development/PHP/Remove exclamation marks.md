# Task 

Write function RemoveExclamationMarks which removes all exclamation marks from a given string.

## Solution with logic (comments)

```
<?php
function remove_exclamation_marks($string) {
  // Used function PHP which replace all occurrences of the search string with the replacement string
  return str_replace('!', '', $string);

?>
```
