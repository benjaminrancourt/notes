# Javascript
## ES6
```javascript
# Obtain a subset of an object, using Object Destructuring and Property Shorthand
# Source: https://stackoverflow.com/a/39333479
const object = { a: 5, b: 6, c: 7  };
const subset = (({ a, c }) => ({ a, c }))(object);
console.log(subset); // { a: 5, c: 7 }
```
