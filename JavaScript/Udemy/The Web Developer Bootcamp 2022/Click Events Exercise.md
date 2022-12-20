# Task 

Let's get some practice using `addEventListener`. I've provided you with two buttons, each with an id: `'hello'` and `'goodbye'`.  Your goal is to add a click listener to each button. 

1. When the hello button is clicked, you should console.log "hello"
2. When the goodbye button is clicked, you should console.log "goodbye"

Make sure to use addEventListener!

## Answer
```index.html
const btnHello = document.querySelector('#hello');
const btnGoodbye = document.querySelector('#goodbye');

btnHello.addEventListener ('click',() => {
    console.log("hello");
}); 

btnGoodbye.addEventListener ('click',() => {
    console.log("goodbye");
}); 

```
