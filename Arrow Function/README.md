```markdown
# Arrow Functions in JavaScript

## Overview

This document provides an example of using arrow functions in JavaScript. Arrow functions offer a concise syntax and are often used for function expressions.

## Code Description

### Arrow Function with Block

```javascript
const hello = (name) => {
    const say = `Hello ${name} <br>`;
    document.writeln(say);
}

hello("Nazmi");
hello("Hakim");
```

- This arrow function takes a single parameter `name`.
- It constructs a greeting message and writes it to the document using `document.writeln`.

### Arrow Function Without Block

```javascript
const sayHello = (name2) => document.writeln(`Hello ${name2} <br>`);
sayHello("Teramoz");
```

- This arrow function also takes a single parameter `name2`.
- It directly returns the greeting message without using a block.

### Arrow Function Return Value

```javascript
const sum = (first, second) => first + second;
document.writeln(sum(1,4), "<br>");
```

- This arrow function takes two parameters, `first` and `second`.
- It returns their sum and writes it to the document.

### Arrow Function Without Parentheses

```javascript
const sayHello2 = name3 => document.writeln(`Hello ${name3} <br>`);
sayHello2("Gatsu");
```

- This arrow function has a single parameter `name3` without parentheses.
- It writes the greeting message to the document.

### Arrow Function as Parameter

```javascript
function giveMeName(callback) {
    callback("Nadea");
}

giveMeName((name4) => document.writeln(`Hello ${name4}`));
```

- The `giveMeName` function takes a callback function as a parameter.
- It calls the callback function with the name `"Nadea"`, which is then used to write a greeting message to the document.

## Usage

To see these arrow functions in action, copy and paste the JavaScript code into an HTML file and open it in a web browser.
