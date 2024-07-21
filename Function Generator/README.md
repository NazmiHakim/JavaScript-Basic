```markdown
# Function Generator Example

This project demonstrates the use of JavaScript function generators with various examples.

## Description

This HTML file contains three examples of function generators in JavaScript:

1. **Basic Function Generator**: Generates a series of names.
2. **Complex Function Generator**: Generates odd numbers up to a specified value.
3. **Lazy Generator**: Generates odd numbers up to a specified value with lazy evaluation, printing a message for each iteration.

## Code Overview

### Basic Function Generator

The `createNames` generator yields three names: "Nazmi", "Hakim", and "Teramoz". These names are written to the document using a `for...of` loop.

```javascript
function* createNames() {
    yield "Nazmi<br>";
    yield "Hakim<br>";
    yield "Teramoz<br>";
}

const names = createNames();
for (const name of names) {
    document.writeln(name);
}
```

### Complex Function Generator

The `ganjil` generator function yields all odd numbers up to a specified value (`value`). These numbers are written to the document using a `for...of` loop.

```javascript
function* ganjil(value) {
    for (let i = 1; i <= value; i++) {
        if (i % 2 === 1) {
            yield i;
        }
    }
}

const angkaGanjil = ganjil(100);
for (const angka of angkaGanjil) {
    document.writeln(angka, "<br>");
}
```

### Lazy Generator

The `buatGanjil` generator function is similar to the `ganjil` function but includes a lazy evaluation that prints a message for each loop iteration. The `.next()` method is used to retrieve the next value from the generator.

```javascript
function* buatGanjil(value) {
    for (let i = 1; i <= value; i++) {
        if (i % 2 === 1) {
            document.writeln(`Loop ${i}<br>`);
            yield i;
        }
    }
}

const angkaGanjil1 = buatGanjil(100);
document.writeln(angkaGanjil1.next().value + "<br>");
document.writeln(angkaGanjil1.next().value + "<br>");
document.writeln(angkaGanjil1.next().value + "<br>");
```
