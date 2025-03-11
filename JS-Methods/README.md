## JavaScript Methods

### Array .from()
```js
const username = "dcode";
const usernameAsArray = Array.from(username, char =>{ return char.toUpperCase()});
console.log(usernameAsArray);

// Result: [ "D", "C", "O", "D", "E" ]
```

### .filter() method 
```js
const items = [
    { name: 'Bike', price: 100 },
    { name: 'TV', price: 200 },
    { name: 'Album', price: 10 },
    { name: 'Book', price: 5 },
    { name: 'Phone', price: 500 },
    { name: 'Computer', price: 1000 },
    { name: 'Keyboard', price: 25 }
];

const filteredItems = items.filter(({ price }) => {  // Destructure price here
    return price <= 100; 
});

console.log(filteredItems);
```
