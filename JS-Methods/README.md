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

const filteredItems = items.filter(({ price }) => {

// Destructure price here
    return price <= 100; 
});

console.log(filteredItems);

/*
Result:
[
  { name: 'Bike', price: 100 },
  { name: 'Album', price: 10 },
  { name: 'Book', price: 5 },
  { name: 'Keyboard', price: 25 }
]
*/
```

### .map() method
map() is about creating a new array by transforming the values of an existing array.
```js
const numbers = [1, 2, 3, 4, 5];

const squaredNumbers = numbers.map(number => number * number);

console.log(squaredNumbers); // Output: [1, 4, 9, 16, 25]
```

### .forEach() method
forEach() is a method in JavaScript that allows you to iterate over the elements of an array. 
```js
const nums = [1, 2, 3, 4, 5];

numbers.forEach((number) =>{
  console.log(number * 2);
}); 
```

## .find() method
find() is a method in JavaScript that's used to search for a specific element within an array. 
```js
const numbers = [10, 5, 20, 8, 15];

const foundNumber = numbers.find(number => number > 10);

console.log(foundNumber); // Output: 20

const notFoundNumber = numbers.find(number => number > 100);

console.log(notFoundNumber); // Output: undefined
```

## .some() method
some() is a JavaScript array method that tests whether at least one element in the array passes the test implemented by the provided function
```js
const numbers = [1, 3, 5, 7, 9];

const hasEvenNumber = numbers.some(number => number % 2 === 0);

console.log(hasEvenNumber); // Output: false

const hasNumberGreaterThanFive = numbers.some(number => number > 5);

console.log(hasNumberGreaterThanFive); // Output: true
```

