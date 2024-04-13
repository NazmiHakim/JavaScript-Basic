---

# Nullish Coalescing Operator

The Nullish Coalescing Operator (`??`) is a JavaScript feature introduced in ECMAScript 2020. It provides a concise syntax for handling default values when dealing with nullable or undefined variables.

## Usage

Consider the following example:

```javascript
let parameter;

let data = parameter ?? "Default Value";

console.log(data); // Output: "Default Value"
```

In this example, `parameter` is `undefined`. When using the Nullish Coalescing Operator (`??`), if the left-hand side operand (`parameter` in this case) evaluates to `null` or `undefined`, the right-hand side operand (`"Default Value"`) is returned instead. If the left-hand side operand is any other falsy value such as `0` or an empty string, it is not considered `null` or `undefined`, and the left-hand side operand is returned.

## Why Use Nullish Coalescing Operator?

1. **Clearer Intent**: It explicitly states that you want to use a default value only when the variable is `null` or `undefined`, which can make the code more readable and less error-prone.

2. **Avoiding Falsy Values**: Unlike the logical OR (`||`) operator, which also provides a way to set default values, the Nullish Coalescing Operator does not consider falsy values such as `0`, `''`, or `false` as indicating a missing value. This ensures that default values are only applied to `null` or `undefined` variables, making it more predictable in certain scenarios.

---
