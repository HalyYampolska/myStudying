# Task 

I've provided you with some simple markup in index.html.  Your task is to use `querySelector` and `querySelectorAll` to select some of those elements.

1. Select all elements that have the class of `"done"` and save them in a variable called `doneTodos`.
2. Select the one checkbox and save it in a variable called `checkbox`. Be careful, there is more than one input element on the page! You'll need to select using the type attribute. (if you can't remember the css attribute selector...google it! That's what I would do!)

```
<!DOCTYPE html>
<html>

<head>
    <title>Todos</title>
</head>

<body>
    <h1>Garden Todos</h1>
    <input type="text" placeholder="New Todo">
    <ul>
        <li>Start Seedlings</li>
        <li class="done">Deadhead Zinnias</li>
        <li class="done">Water Tomatoes</li>
        <li class="done">Harvest Potatoes</li>
        <li>Prune Roses</li>
    </ul>
    <label>Delete All</label>
    <input type="checkbox" id="scales" name="scales" checked>

</body>

</html>
```

app.css
```
/* No need to change anythign in here! */
.done {
    color: grey;
    text-decoration: line-through;
}
```

## Answer

```javascript
const doneTodos = document.querySelectorAll ('.done');
const checkbox = document.querySelector ('#scales');
```
