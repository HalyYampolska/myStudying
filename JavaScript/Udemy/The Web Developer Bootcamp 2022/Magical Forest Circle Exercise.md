# Task 

I've provided you with some basic markup in `index.html`.  Please do not change any of the markup directly.  Instead, use JavaScript to make the following changes:

1. Select the div with the id of `container`.  Using JavaScript, set it's text alignment to 'center';
2. Select the image and use JavaScript to give it a width of 150px and a border radius of 50%

```
<!DOCTYPE html>

<head>
    <title>Forest</title>
    <!--LEAVE THESE LINES ALONE, PLEASE! THEY MAKE THE LIVE PREVIEW WORK!-->
    <script src="node_modules/babel-polyfill/dist/polyfill.js" type="text/javascript"> </script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

</head>

<body>
   <div id="container">
        <h1>I &hearts; Trees</h1>
        <img src="https://images.unsplash.com/photo-1596328546171-77e37b5e8b3d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1400&q=80" alt="">
    </div>
</body>

</html>
```
`

## Answer

```javascript
let mainCont = document.querySelector('#container');
mainCont.style.textAlign = 'center';

let mainImg = document.querySelector('img');
mainImg.style.width = '150px';
mainImg.style.borderRadius = '50%';
```
