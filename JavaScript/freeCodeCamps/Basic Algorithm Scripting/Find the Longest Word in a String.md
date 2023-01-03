# Task

Return the length of the longest word in the provided sentence.

Your response should be a number.

 ## Before

```javascript
function findLongestWordLength(str) {
  return str.length;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");
```

## After

### 1
```javascript
function findLongestWordLength(str) {
  var strSplit = str.split(' ');
  var longestWord = 0;
  for(var i = 0; i < strSplit.length; i++){
    if(strSplit[i].length > longestWord){
	longestWord = strSplit[i].length;
     }
  }
  return longestWord;
}


findLongestWordLength("The quick brown fox jumped over the lazy dog");
```

### 2
```javascript
function findLongestWordLength(str) {
  var longestWord = str.split(' ').sort(function(a, b) { return b.length - a.length; });
  return longestWord[0].length;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");
```

### 3
```javascript
function findLongestWordLength(str) {
    var longestWord = str.split(' ').reduce(function  (longest, nextWord) {
    return nextWord.length > longest.length ? nextWord : longest;
  }, "");
    return longestWord.length;
}
findLongestWordLength("The quick brown fox jumped over the lazy dog");
```
