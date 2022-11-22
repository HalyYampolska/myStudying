# Task 

Define an object called `square`, which will hold methods that have to do with the geometry of squares. It should contain two methods, `area` and `perimeter` 

1. `area` should accept the length of a `side` (all sides are the same in a square) and then return the side squared. 

2. `perimeter` should accept the length of a `side` and return that side multiplied by 4.

```javascript
square.area(10) //100
square.perimeter(10) //40

```

## Answer

```javascript
const square = {
    area (side) {
        return (side * side);
    },
    perimeter (side) {
        return (side * 4);
    }
}
```
