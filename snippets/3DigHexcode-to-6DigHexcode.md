### 3DigHexcode to 6DigHexcode

Use `Array.map()` to map the array created by `String.split()` and `Array.join()` to join 
the mapped array for converting a three-digit RGB notated hexadecimal colorcode to the six-digit form. 

```js
const convertHex = shortHex => 
  shortHex[0] == '#' ? ('#' + shortHex.slice(1).split('').map(x => x+x).join('')) : 
    ('#' + shortHex.split('').map(x => x+x).join(''))
// convertHex('#03f') -> '#0033ff'
// convertHex('05a') -> '#0055aa'
```
