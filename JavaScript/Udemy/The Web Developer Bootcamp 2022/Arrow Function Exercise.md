# Task 

Write an arrow function expression called `greet`.  It should accept a single string argument, representing a person's name.  It should return a greeting string as shown below:

```javascript
greet("Hagrid") //"Hey Hagrid!" 
greet("Luna") //"Hey Luna!"
```

## Answer

```javascript
const greet = (name) => {
    return "Hey " + name + "!";
}
```
