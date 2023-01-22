### The Second Challenge 

Convert the given number into a roman numeral.

| Roman numerals  | Arabic numerals |
| --------------- | --------------- |
|         M       |       1000      |
|         CM      |       900       |
|         D       |       500       |
|         CD      |       400       |
|         C       |       100       |
|         XC      |       90        |
|         L       |       50        |
|         XL      |       40        |
|         X       |       10        |
|         IX      |       9         |
|         V       |       5         |
|         IV      |       4         |
|         I       |       1         |
	
All roman numerals answers should be provided in upper-case.

## Befor 

```javascript
function convertToRoman(num) {
 return num;
}

convertToRoman(36);
```

## After 

```javascript
function convertToRoman(num) {
// Create a roman numeral to number lookup table 
  const lookupTable = {
    M:	1000,
    CM:	900,
    D:	500,
    CD:	400,
    C:	100,
    XC:	90,
    L:	50,
    XL:	40,
    X:	10,
    IX:	9,
    V:	5,
    IV:	4,
    I:	1
    };
// Create string builder (accumulator)
  let accumulator = '';
// Create loop
  for (const key in lookupTable) {
    const numVal = lookupTable[key];
// While (currentNum <= num) subtract currentNum from num and after that add the symbol to the accumulator 
    while (numVal <= num) {
      num -= numVal;
      accumulator += key;
    }   
  }
// Return accumulator
 return accumulator;
}

convertToRoman(36);
```
