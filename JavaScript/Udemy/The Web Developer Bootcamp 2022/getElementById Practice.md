# Task 

Let's get some practice using `getElementById`. I've provided a little bit of markup for you (please don't change it!)  Your goal is to write code in `app.js` to select the following elements using getElementById:

1. Select the image element by its id and save it to a variable called `image`

2. Select the h1 by its id and save it to a variable called `heading`

Note: You may need to reset the code before attempting this exercise

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unicorn</title>
</head>
<body>
    <h1 id="mainheading">I &hearts; unicorns</h1>
    <img src="https://devsprouthosting.com/images/unicorn.jpg" id="unicorn" alt="unicorn">
</body>
</html>
```

## Answer

```javascript
const image = document.getElementById('unicorn');
const heading = document.getElementById('mainheading');
```
