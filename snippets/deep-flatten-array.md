### Deep flatten array

Use recursion.
Use `reduce()` to get all elements that are not arrays, flatten each element that is an array.

```js
const deepFlatten = arr =>
  arr.reduce( (a, v) => a.concat( Array.isArray(v) ? flatten(v) : v ), []);
// deepFlatten([1,[2],[[3],4],5]) -> [1,2,3,4,5]
```
