
```
<?php
// Declaration of a function with two variables (the list where we are looking and the number we are looking for).
function binary_search($list, $item) {
    // Шnitializeв 2 variables, $low and $high. $low is set to the beginning of the array (index 0), and $high is set to the end of the array
    $low = 0;
    $high = count($list) - 1;
    // Binary code loop condition. Executes as long as `$low` is less than or equal to `$high`.
    while ($low <= $high) {
        // Сalculateв the middle of the list.
        $mid = (int)(($low + $high) / 2);
        // Retrieves an element from `$list` at index `$mid` and stores it in the `$guess` variable.
        $guess = $list[$mid];
        // Checking if the element (`$guess`) matches the desired element (`$item`)
        if ($guess == $item) {
            return $mid;
          // Update range boundaries
        } elseif ($guess > $item) {
            $high = $mid - 1;
        } else {
            $low = $mid + 1;
        }
    }

    return null;
}
?>
```
