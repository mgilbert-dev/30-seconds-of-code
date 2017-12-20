### stringToArrayOfWords

Converts a given string into an array of words

Use `String.split(/[\W_]+/)` to convert the string to an array with the use of regex.

```js
const stringToArrayOfWords = (str, pattern = /[\W_]+/) => str.split(pattern).filter(Boolean)

// stringToArrayOfWords("I love javaScript!!") -> ["I", "love", "javaScript"]
// stringToArrayOfWords("python, javaScript & coffee") -> ["python", "javaScript", "coffee"]
```