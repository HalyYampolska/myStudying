# Task 

An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.

Example: (Input --> Output)

"Dermatoglyphics" --> true "aba" --> false "moOse" --> false (ignore letter case)
```
isIsogram "Dermatoglyphics" = true
isIsogram "moose" = false
isIsogram "aba" = false
```

## Solution with logic (comments)

```
<?php
function isIsogram($string) {
    $string = strtolower($string); // Make characters lowercase
    $uniqueCharCount = array(); 

    for ($i = 0; $i < strlen($string); $i++) {
        $char = $string[$i];
        if (isset($uniqueCharCount[$char])) {
            return false; // If character is duplicate
        }
        $uniqueCharCount[$char] = true;
    }

    return true; // All characters are unique
}
?>
```
