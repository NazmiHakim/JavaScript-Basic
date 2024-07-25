# Destructuring in JavaScript

This project demonstrates various ways of using destructuring in JavaScript. Destructuring is a convenient way of extracting multiple values from data stored in (possibly nested) objects and arrays. This README will guide you through the examples provided in the HTML file.

## Examples

### Fetching Data Manually

We start by manually extracting values from an array:

```javascript
const names = ["Nazmi", "Hakim", "Teramoz"];
const firstName = names[0];
const middleName = names[1];
const lastName = names[2];

console.info(firstName);  // Output: Nazmi
console.info(middleName); // Output: Hakim
console.info(lastName);   // Output: Teramoz
```

### Destructuring Arrays

Destructuring makes it easier to extract multiple values from arrays:

```javascript
const names2 = ["Gatsu", "Galuh", "Terra", "Nazmi", "Hakim"];
const [firstName2, middleName2, lastName2, ...others] = names2;

console.info(firstName2);  // Output: Gatsu
console.info(middleName2); // Output: Galuh
console.info(lastName2);   // Output: Terra
console.info(others);      // Output: ["Nazmi", "Hakim"]
```

### Fetching Data from an Object

Extracting values from an object manually:

```javascript
const person = {
    firstName3: "Nazmi",
    lastName3: "Hakim",
    address: {
        street: "Jl. Manarap",
        city: "Banjarmasin",
        country: "Indonesia",
    },
    hobby: "Game",
    age: "19"
};
```

### Destructuring Objects

Destructuring allows extracting multiple values from objects:

```javascript
let { firstName3, lastName3, address, ...others2 } = person;

console.info(firstName3);  // Output: Nazmi
console.info(lastName3);   // Output: Hakim
console.info(address);     // Output: { street: "Jl. Manarap", city: "Banjarmasin", country: "Indonesia" }
console.info(others2);     // Output: { hobby: "Game", age: "19" }
```

### Destructuring Nested Objects

Destructuring also works with nested objects:

```javascript
const { firstName3, lastName3, address: { country, city, street }, ...others2 } = person;

console.info(firstName3);  // Output: Nazmi
console.info(lastName3);   // Output: Hakim
console.info(country);     // Output: Indonesia
console.info(city);        // Output: Banjarmasin
console.info(street);      // Output: Jl. Manarap
console.info(others2);     // Output: { hobby: "Game", age: "19" }
```

### Destructuring in Function Parameters

You can destructure objects directly in function parameters:

#### Example 1:

```javascript
function displayPerson({ firstName, middleName, lastName }) {
    console.info(firstName);  // Output: Nazmi
    console.info(middleName); // Output: Teramoz
    console.info(lastName);   // Output: Gatsu
}

const person = {
    firstName: "Nazmi",
    middleName: "Teramoz",
    lastName: "Gatsu"
};

displayPerson(person);
```

#### Example 2:

```javascript
function sum([first, second]) {
    return first + second;
}

console.info(sum([10, 10]));  // Output: 20
console.info(sum([20, 10]));  // Output: 30
```

### Default Values in Destructuring Arrays

You can set default values when destructuring arrays:

```javascript
const names = ["Nazmi", 'Teramoz'];
const [firstName, middleName, lastName = "Gatsu"] = names;

console.info(firstName);  // Output: Nazmi
console.info(middleName); // Output: Teramoz
console.info(lastName);   // Output: Gatsu
```

### Default Values in Destructuring Objects

Setting default values and using other variable names while destructuring objects:

```javascript
const person = {
    firstName: "Nazmi",
    lastName: "Gatsu"
};

const { firstName, middleName = "Teramoz", lastName } = person;
console.info(firstName);  // Output: Nazmi
console.info(middleName); // Output: Teramoz
console.info(lastName);   // Output: Gatsu

// Using other variable names
const {
    firstName: frontName,
    middleName: midName = "Teramoz",
    lastName: backName
} = person;

console.info(frontName);  // Output: Nazmi
console.info(midName);    // Output: Teramoz
console.info(backName);   // Output: Gatsu
```

## Conclusion

This HTML file showcases various examples of how to use destructuring in JavaScript for arrays and objects, including nested objects and default values. Destructuring is a powerful feature that can make your code cleaner and more readable.
