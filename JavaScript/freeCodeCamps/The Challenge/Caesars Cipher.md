### The Third Challenge 

One of the simplest and most widely known ciphers is a Caesar cipher, also known as a shift cipher. In a shift cipher the meanings of the letters are shifted by some set amount.

A common modern use is the ROT13 cipher, where the values of the letters are shifted by 13 places. Thus `A ↔ N`, `B ↔ O` and so on.

Write a function which takes a ROT13 encoded string as input and returns a decoded string.

All letters will be uppercase. Do not transform any non-alphabetic character (i.e. spaces, punctuation), but do pass them on.

## Befor 

```javascript
function rot13(str) {
  return str;
}

rot13("SERR PBQR PNZC");
```

## After 

```javascript
function rot13(str) {
  // Create alphabet
  const alphabet = [
    "A",
    "B",
    "C",
    "D",
    "E",
    "F",
    "G",
    "H",
    "I",
    "J",
    "K",
    "L",
    "M",
    "N",
    "O",
    "P",
    "Q",
    "R",
    "S",
    "T",
    "U",
    "V",
    "W",
    "X",
    "Y",
    "Z"];
  
  // Create accumulator
  let accumulator = "";
  // Create loop
  for (let i = 0; i < str.length; i++) {
      
      // if char is not letter just push to accumulator)
      const char = str[i];
      const isCharLetter = alphabet.includes(char);
      
      if (isCharLetter === false) {
          accumulator += char;
      } else {
      // else coutn "+" or "-" 13 (ROT13) adn add to accumulator) 
          const charIndex = alphabet.findIndex((c) => c === char); // this return A => 0, Z => 25
      
          accumulator += alphabet[charIndex + 13] || alphabet[charIndex - 13];            
      }
  }
  // return ouput    
  return  accumulator;
}

rot13("SERR PBQR PNZC");
```
