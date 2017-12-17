### Take every nth element

Use `Array.filter()` to create a new array that contains every nth element of a given array.

```js
const everyNth = (arr, nth) => arr.filter((e, i) => i % nth === 0);
// everynth([1,2,3,4,5,6], 2) -> [ 1, 3, 5 ]
```
