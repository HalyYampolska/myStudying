# Task 

Finish the solution so that it sorts the passed in array of numbers. If the function passes in an empty array or null/nil value then it should return an empty array.

For example:
```
solution([1, 2, 10, 50, 5]); // should return [1,2,5,10,50]
solution(null); // should return []
```

## Solution with logic (comments)

```
<?php
function solution($nums) {
  // Check if the input array is null or empty
  if ($nums === null || count($nums) === 0) {
    return [];
  }
  // Sort the array
  sort($nums);

  return $nums;
}
?>
```
