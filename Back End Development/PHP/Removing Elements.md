# Task 

Take an array and remove every second element from the array. Always keep the first element and start removing with the next element.

Example:
```
["Keep", "Remove", "Keep", "Remove", "Keep", ...] --> ["Keep", "Keep", "Keep", ...]
```

None of the arrays will be empty, so you don't have to worry about that!

## Solution with logic (comments)

```
<?php
function removeEveryOther($array) { // Take a massive
    $result = array(); // Create a new massive for new massive
    $firstword = true; // Create a variable for rangering 

    foreach ($array as $element) { // Iterates through the elements of the input array
        if ($firstword) { // If the conditional variable is true, then the current element should be left
            $result[] = $element; // Add ti a new massive if true 
        }
        $firstword = !$firstword; // After each iteration of the loop, we toggle the value to decide whether to keep the next element.
    }

    return $result;
}
?>
```
