# Task 

Complete the function that takes two integers (`a`, `b`, where `a < b`) and return an array of all integers between the input parameters, including them.

For example:
`
a = 1
b = 4
--> [1, 2, 3, 4]
`
```
function between(int $a, int $b): array {
    return [];
}
```

## Logic

Function `between` take 2 `int`s  `a` and `b`. 
1. Create empty array for collect int between `a` and `b`.
2. Use `for` collect all int in one array.
3. Return array.  

## Solution

```
<?php
function between(int $a, int $b): array {
  // Create an emply array for all int between $a and $b
  $result = [];
  // Create condition for check all int between $a and $b
    for ($i = $a; $i <= $b; $i++) {
      // All int between $a and $b collect here
        $result[] = $i;
    }
    return $result;
}
?>
```
