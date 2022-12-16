# Task 

I've provided you with an `<h1>` element which contains 7 individual spans (each holding a single letter). 

1. Please write some JavaScript to make them rainbow-colored!
2. In app.js you'll find an array of `color` names called colors.  It looks like: `['red', 'orange', 'yellow', 'green', 'blue', 'indigo', 'violet']`.
3. Your task is to select all spans, iterate over them, and assign them each one of the colors from the colors array.  The first span should be red, the second should be orange, etc.

```
<!DOCTYPE html>

<head>
    <title>Rainbow</title>
    <!--LEAVE THESE LINES ALONE, PLEASE! THEY MAKE THE LIVE PREVIEW WORK!-->
    <script src="node_modules/babel-polyfill/dist/polyfill.js" type="text/javascript"> </script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

</head>

<body>
    <!--DON'T TOUCH THIS FILE PLEASE!-->
    <h1>
        <span>R</span>
        <span>A</span>
        <span>I</span>
        <span>N</span>
        <span>B</span>
        <span>O</span>
        <span>W</span>
    </h1>
</body>

</html>
```

## Answer

```javascript
const colors = ['red', 'orange', 'yellow', 'green', 'blue', 'indigo', 'violet']; //PLEASE DON'T CHANGE THIS LINE!

//YOU CODE GOES HERE:
const spans = document.querySelectorAll('h1 span');
spans.forEach((letter, color) => {
  letter.style.color = colors[color];
});
```
