# Introduction

The last challenge showed how the `@for` directive uses a starting and ending value to loop a certain number of times. Sass also offers the `@each` directive which loops over each item in a list or map. On each iteration, the variable gets assigned to the current value from the list or map.
```
@each $color in blue, red, green {
  .#{$color}-text {color: $color;}
}
```
A map has slightly different syntax. Here's an example:
```
$colors: (color1: blue, color2: red, color3: green);

@each $key, $color in $colors {
  .#{$color}-text {color: $color;}
}
```
Note that the `$key` variable is needed to reference the keys in the map. Otherwise, the compiled CSS would have `color1`, `color2`... in it. Both of the above code examples are converted into the following CSS:
```
.blue-text {
  color: blue;
}

.red-text {
  color: red;
}

.green-text {
  color: green;
}
```

# Task 

Write an `@each` directive that goes through a list: `blue, black, red` and assigns each variable to a `.color-bg` class, where the `color` part changes for each item. Each class should set the `background-color` the respective color.

## Before

```
<style type='text/scss'>



  div {
    height: 200px;
    width: 200px;
  }
</style>

<div class="blue-bg"></div>
<div class="black-bg"></div>
<div class="red-bg"></div>
```


## After

```
<style type='text/scss'>
  @each $color in blue, black, red {
    .#{$color}-bg {background-color: $color;}
  }
  
  div {
    height: 200px;
    width: 200px;
  }



  div {
    height: 200px;
    width: 200px;
  }
</style>

<div class="blue-bg"></div>
<div class="black-bg"></div>
<div class="red-bg"></div>
```
