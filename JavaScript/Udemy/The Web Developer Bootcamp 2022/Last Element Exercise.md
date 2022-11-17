# Task 

Please write a function called `lastElement` which accepts a single array argument.  The function should return the last element of the array (without removing the element).  If the array is empty, the function should return `null`.

lastElement([3,5,7]) //7
lastElement([1]) //1
lastElement([]) //null


## Answer

```javascript
function lastElement(arr) {
    if (arr.length > 0) {
        return arr[arr.length - 1];
    } 
    return null;   
}
```
