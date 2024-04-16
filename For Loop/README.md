```
# For Loop Examples

This repository contains examples of using for loops in JavaScript.

## For Loop With Condition

The first example demonstrates a for loop with the condition placed within the loop declaration.

```javascript
let counter = 1;
for (; counter <= 10;) {
    document.writeln(`<p>${counter}</p>`);
    counter++;
}
```

In this loop:
- `counter` is initialized before the loop.
- The loop continues as long as `counter` is less than or equal to 10.
- After each iteration, the `counter` is incremented by 1.

## For Loop With Init Statement

The second example showcases a for loop with the initialization statement included in the loop declaration.

```javascript
for (let counter2 = 1; counter2 <= 10;) {
    document.writeln(`<p>${counter2}</p>`);
    counter2++;
}
```

In this loop:
- `counter2` is initialized within the loop declaration.
- The loop continues as long as `counter2` is less than or equal to 10.
- After each iteration, the `counter2` is incremented by 1.

## Conclusion

Both examples achieve the same result, demonstrating the flexibility of for loops in JavaScript. Developers can choose the structure that best fits their coding style and requirements.
