# Falsy and Truthy

This repository contains a simple JavaScript script that demonstrates the concept of falsy and truthy values in JavaScript.

## Overview

In JavaScript, values are inherently considered either "falsy" or "truthy" when evaluated in a boolean context. Understanding these concepts is crucial when writing conditionals or evaluating expressions in JavaScript.

### Falsy Values

The following values are considered falsy in JavaScript:
- `false`: The boolean value `false`.
- `0`, `-0`: The number zero and negative zero.
- `""`, `''`, ``: All empty strings.
- `null`: The null value.
- `undefined`: The undefined value.
- `NaN`: Not a Number.

### Truthy Values

Conversely, the following values are considered truthy in JavaScript:
- `true`: The boolean value `true`.
- Non-empty strings: Any string with at least one character.
- Non-zero numbers: Any non-zero numerical value.
- Non-null and non-undefined values: Any value other than null or undefined.
- `NaN`: Although considered falsy, `NaN` behaves differently when evaluated in certain contexts, such as comparison operators.

## Usage

To understand how JavaScript treats falsy and truthy values, simply run the provided script in a JavaScript environment. The script evaluates the truthiness of various data types and prints the result to the screen.

## Example

```javascript
let data;
if (data){
    document.writeln("TRUE")
} else {
    document.writeln("FALSE")
}

let data2 = "FALSE";
if (data2){
    document.writeln("TRUE")
} else {
    document.writeln("FALSE")
}
```

In this example, data is undefined, so it is considered falsy, while data2 contains a non-empty string, making it truthy.
