# Task 

Without touching `index.html`, please use JavaScript to create exactly 100 new button elements! Add each new button inside the container element provided in index.html.  Unfortunately, Udemy's exercise tool does not support to the append method, so you will need to use appendChild.  Here are the steps:

1. Create exactly 100 new button elements
2. Each button must have some text inside of it (it doesn't matter what)
3. Each button must be appended inside the container div.

Hint: Loop 100 times. Inside the loop, create a new empty button element.  Add some innerText to the button.  Use appendChild to add the button to the container.

```
<!DOCTYPE html>

<head>
    <title>100 Buttons!</title>
</head>

<body>
    <!--DO NOT TOUCH THIS FILE PLEASE!-->
    <h1>Look At All My Buttons!</h1>
    <div id="container">
    
    </div>
</body>

</html>
```

## Answer

```javascript
const div = document.querySelector('div');

for (let i = 0; i < 100; i++) {
    const button = document.createElement('button');
    button.innerText= "Hey!";
    div.appendChild(button);
}
```
