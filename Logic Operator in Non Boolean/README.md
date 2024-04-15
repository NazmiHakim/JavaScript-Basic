
```
# Non-Boolean Logic Operators in JavaScript

This document outlines how logical operators (|| and &&) function in JavaScript when applied to non-boolean values.

## OR (||) Operator in Non-Boolean Context

The OR operator (||) in JavaScript can be used with non-boolean values. It behaves as follows:

- It evaluates the expressions from left to right.
- It returns the first truthy value encountered.
- If none of the expressions are truthy, it returns the last value.

### Examples:

```javascript
console.info("Hello" || ""); // Outputs: Hello
console.info("" || []); // Outputs: []
console.info("0" || "ZERO"); // Outputs: 0
console.info(0 || "ZERO"); // Outputs: ZERO
console.info(null || "NULL"); // Outputs: NULL
console.info(undefined || "UNDEFINED"); // Outputs: UNDEFINED

const person = {
    firstName: "",
    lastName: "Hakim",
};

const name = person.firstName || person.lastName;
console.info(name); // Outputs: Hakim
```

## AND (&&) Operator in Non-Boolean Context

The AND operator (&&) in JavaScript can also be used with non-boolean values. Its behavior is as follows:

- It evaluates the expressions from left to right.
- It returns the first falsy value encountered.
- If none of the expressions are falsy, it returns the last value.

### Examples:

```javascript
console.info("Hello" && ""); // Outputs: ""
console.info("" && []); // Outputs: ""
console.info("0" && "ZERO"); // Outputs: ZERO
console.info(0 && "ZERO"); // Outputs: 0
console.info(null && "NULL"); // Outputs: null
console.info(undefined && "UNDEFINED"); // Outputs: undefined
console.info("undefined" && "null"); // Outputs: null
```

These examples demonstrate how logical operators behave when dealing with non-boolean values in JavaScript.

Feel free to adjust or expand upon it as needed!
