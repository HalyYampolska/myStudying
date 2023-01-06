# Introduction

Constructors are functions that create new objects. They define properties and behaviors that will belong to the new object. Think of them as a blueprint for the creation of new objects.

Here is an example of a constructor:
```javascript
function Bird() {
  this.name = "Albert";
  this.color = "blue";
  this.numLegs = 2;
}
```
This constructor defines a `Bird` object with properties `name`, `color`, and `numLegs` set to `Albert`, `blue`, and `2`, respectively. Constructors follow a few conventions:

1. Constructors are defined with a capitalized name to distinguish them from other functions that are not constructors.
2. Constructors use the keyword this to set properties of the object they will create. Inside the constructor, this refers to the new object it will create.
3. Constructors define properties and behaviors instead of returning a value as other functions might.

## Task 

Create a constructor, `Dog`, with properties `name`, `color`, and `numLegs` that are set to a string, a string, and a number, respectively.

## Before

```javascript

```

## After

```javascript
function Dog() {
  this.name = "Albert";
  this.color = "tan";
  this.numLegs = 4;
}
```
