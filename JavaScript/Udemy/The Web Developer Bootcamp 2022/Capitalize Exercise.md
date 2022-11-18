# Task 

Define a function called `capitalize` that accepts a string argument and returns a new string with the first letter capitalized (but the rest of the string unchanged).  
For example:

```javascript
capitalize('eggplant') // "Eggplant"
capitalize('pamplemousse') // "Pamplemousse"
capitalize('squid') //"Squid"
```
##Hints

1. Remember that strings are immutable, meaning that you cannot simply change the first letter in the original string.  You will need to make a new string that you return.
2. Single out the first letter and capitalize it. (use a string method to help!)
3. Add that first letter to the rest of the original string, sliced to omit the original first letter (use a string method to help!)
For example: 'eggplant' becomes 'E' + 'ggplant'

## Answer

```javascript
var string = "";

function capitalize (str) {
    return str.charAt(0).toUpperCase() + str.slice(1);
}
```

###Thinking

1. We need declare a variable. 
2. Use charAt() method to select the first character of str.
3. For convert use toUpperCase(). 
4. Use the slice() method and get the remainder of the string.
5. We need function that accepts a str as only argument and returns result.    
