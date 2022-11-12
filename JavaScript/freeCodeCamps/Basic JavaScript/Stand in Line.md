# Introduction
In Computer Science a `queue` is an abstract `Data Structure` where items are kept in order. New items can be added at the back of the queue and old items are taken off from the front of the queue.

## Task
Write a function `nextInLine` which takes an array (`arr`) and a number (`item`) as arguments.
Add the number to the end of the array, then remove the first element of the array.
The `nextInLine` function should then return the element that was removed.

```javascript
function nextInLine(arr, item) {
  // Only change code below this line

  // Only change code above this line
}

// Setup
let testArr = [1, 2, 3, 4, 5];

// Display code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6));
console.log("After: " + JSON.stringify(testArr));

```

## Answer

```javascript
  var pushItem = arr.push(item);
  var removedItem = arr.shift();
  return removedItem;
```

#### Step by step 
1. For add number at the end of the array use `.push()`
2. For remove first element use `.shift()`
3. For return element what was removed use`return removeItem`
