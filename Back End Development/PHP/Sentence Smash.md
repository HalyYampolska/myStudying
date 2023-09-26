# Task 

Write a function that takes an array of words and smashes them together into a sentence and returns the sentence. You can ignore any need to sanitize words or add punctuation, 
but you should add spaces between each word. Be careful, there shouldn't be a space at the beginning or the end of the sentence!

Example
```
['hello', 'world', 'this', 'is', 'great']  =>  'hello world this is great'
```

## Solution with logic (comments)

```
<?php
function smash(array $words): string {
  // Used WP method. ' ' guarantee gap between worlds 
  $result = implode(' ', $words);
  return $result;
}
?>
```
