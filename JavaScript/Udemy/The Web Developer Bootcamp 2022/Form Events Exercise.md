# Task 

Time to get some practice working with forms and form events! `index.html` already has a form element that contains two `<input>` elements, one for quantity and one for a product name.  `index.html` also contains an empty `<ul>` where you will append new `<li>`s.  Watch the gif at the bottom for an overview of how your code should work. Your task is to follow these steps:

1. Listen for the form submission
2. When the form is submitted, prevent the default behavior
3. Grab the quantity input value and the product input value.
4. Create a new <li> element.  Set the text on the new <li> to include the quantity and product name from the form.
5. Append the new <li> to the <ul> on the page
6. Reset the inputs

Please note:
1. Udemy's interface does not yet recognize some of the newer JS syntax, e.g., .append()
You will need to use alternate (older) syntax for this method in order to get the tests to pass.
2. The form will need to be assigned to a variable named form for the test to pass, I've already included this line of code for you in the app.js code.

```
<!DOCTYPE html>

<head>
    <title>Grocery List</title>
    <!--LEAVE THESE LINES ALONE, PLEASE! THEY MAKE THE LIVE PREVIEW WORK!-->
    <script src="node_modules/babel-polyfill/dist/polyfill.js" type="text/javascript"> </script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

</head>

<body>
    <h1>Grocery List</h1>
    <form action="/nowhere">
        <label for="item">Enter A Product</label>
        <input type="text" id="product" name="product">
        <label for="item">Enter A Quantity</label>
        <input type="number" id="qty" name="qty">
        <button>Submit</button>
    </form>

    <ul id="list"></ul>
</body>

</html>
```

## Answer

```javascript
const form = document.querySelector('form');
const product = document.querySelector ("#product");
const qty = document.querySelector ("#qty");
const list = document.querySelector ("#list");

form.addEventListener("submit", function(e) {
   e.preventDefault();
    const newProduct = product.value;
    const newQty = qty.value;
    const li = document.createElement ("li");
    
    li.innerText = `${newQty} ${newProduct}`;
    list.appendChild(li);
    
    product.value = "";
    qty.value = "";
});
```
