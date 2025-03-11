## Spread Operator Purposes

1. Copying Arrays
```js
const originalArray = [1, 2, 3];
const copiedArray = [...originalArray]; // Creates a new array
copiedArray.push(4);
console.log(originalArray); // [1, 2, 3]
console.log(copiedArray); // [1, 2, 3, 4]
```

2. Concatenating Arrays
```js
const array1 = [1, 2];
const array2 = [3, 4];
const combinedArray = [...array1, ...array2]; // [1, 2, 3, 4]
```

3. Passing Arguments to Functions
```js
function sum(a, b, c) {
    return a + b + c;
}
const numbers = [1, 2, 3];
console.log(sum(...numbers)); // 6
```

4. Converting Strings to Arrays
```js
const str = "hello";
const charArray = [...str]; // ['h', 'e', 'l', 'l', 'o']
```

5. Expanding Objects
```js
const originalObject = { a: 1, b: 2 };
const copiedObject = { ...originalObject };
copiedObject.c = 3;
console.log(originalObject); // { a: 1, b: 2 }
console.log(copiedObject); // { a: 1, b: 2, c: 3 }
```

6. Merging Objects
```js
const object1 = { a: 1, b: 2 };
const object2 = { c: 3, d: 4 };
const mergedObject = { ...object1, ...object2 }; // { a: 1, b: 2, c: 3, d: 4 }
```


