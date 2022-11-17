# Task 

Please help me decide by writing me a function called `isShortsWeather`. 

It should accept a single number argument, which we will call `temperature`. 

If `temperature` is greater than or equal to 75, return `true`. 

Otherwise, return `false`.   

isShortsWeather(80) //true
isShortsWeather(48) //false
isShortsWeather(75) //true

## Answer

```javascript
function isShortsWeather(temperature) {
    if (temperature >= 75) {
        return true;
    } else {
        return false;
    }
    }
```
