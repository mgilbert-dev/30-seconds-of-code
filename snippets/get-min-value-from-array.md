### Get min value from array

Passing an array, it executes the Math.min method using the spread operator to fill its variadic arguments

```js
const getMinValue = arr => Math.min(...arr);
// getMinValue([10, 1, 5) -> 1
```
