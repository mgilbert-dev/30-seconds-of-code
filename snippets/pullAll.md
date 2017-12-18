### pullAll

This method is like pull except that it accepts an array of values to filter out before Mutating and pulling all the values from the original array.

Use `Array.filter()` and `Array.includes()` to pull out the values that are not needed.
Use `Array.length = 0` to mutate the passed in array by resetting it's length to zero and `Array.push()` to re-populate it with only the pulled values.

```js
const pullAll = (arr, pullArr) => {
  let pulled = arr.filter((v, i) => !pullArr.includes(v));
  arr.length = 0;
  pulled.forEach(v => arr.push(v));
}

// let myArray = ['a', 'b', 'c', 'a', 'b', 'c'];
// pullAll(myArray, ['a', 'c']);
// console.log(myArray) -> [ 'b', 'b' ]
```