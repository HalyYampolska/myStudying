# Task 

In this exercise, I'm asking you to write some inline event handlers WHICH IS NOT SOMETHING I RECOMMEND, but hopefully it will illustrate to you just how annoying it can be. In index.html, you'll find an `<h1>` element and a `<button>`.  Please add two inline click handlers directly in the html:

1. When the h1 is clicked, you should print*  "boo"
2. When the button is clicked, you should print "clicked"

* "print" = `console.log('something here')`;

## Answer
```index.html
<body>
    <h1 onclick="alert(console.log('boo'))">Inline Events Suck...</h1>
    <button id="btn" onclick="alert(console.log('clicked'))">Click Me</button>
</body>
```
