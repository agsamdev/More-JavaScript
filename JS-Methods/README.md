## JavaScript Methods

### JavaScript Array .from()
```js
const username = "dcode";
const usernameAsArray = Array.from(username, char =>{ return char.toUpperCase()});
console.log(usernameAsArray);

// Result: [ "D", "C", "O", "D", "E" ]
```
