# Task

Check if a value is classified as a boolean primitive. Return `true` or `false`.

Boolean primitives are `true` and `false`.

 ## Before

```javascript
function booWho(bool) {
  return bool;
}

booWho(null);
```

## After

```javascript
function booWho(bool) {
  return typeof bool === "boolean";
}

booWho(null);
```
