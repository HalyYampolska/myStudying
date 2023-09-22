# Task 

Your function takes two arguments:

- current father's age (years);
- current age of his son (years);
Сalculate how many years ago the father was twice as old as his son (or in how many years he will be twice as old). The answer is always greater or equal to 0, no matter if it was in the past or it is in the future.

## Logic

We have two arguments (`$dad_years_old$dad_years_old` and `$son_years_old`). 
1. Сheck in `always greater or equal to 0`. 
2. Calculate the difference between the father's age and twice the age of the son.
3. Calculate the difference between twice the age of the son and the father's age and return this value.

## Solution

```
<?php
function twice_as_old($dad_years_old, $son_years_old){
  // Check "always greater or equal to 0"
  if ($dad_years_old >= $son_years_old * 2) {
    // Return result if father older
    return $dad_years_old - $son_years_old * 2;
  } else {
    // Return result if father younger
    return $son_years_old * 2 - $dad_years_old;
  }
}
?>
```
