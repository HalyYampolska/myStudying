# Task 

Define an object called `hen`. It should have three properties:

```javascript
`name` should be set to 'Helen'
`eggCount` should be set to 0
`layAnEgg` should be a method which increments the value of `eggCount` by 1 and returns the string "EGG".  You'll need to use `this`.
```

```javascript
hen.name // "Helen"
hen.eggCount // 0
hen.layAnEgg() // "EGG"
hen.layAnEgg() // "EGG"
hen.eggCount // 2
```

## Answer

```javascript
const hen = {
    name: "Helen",
    eggCount: 0,
    layAnEgg() {
        this.eggCount++;
        return "EGG";
    }
}
```
