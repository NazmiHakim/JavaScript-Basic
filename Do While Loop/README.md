```
# Do While Loop Example

This example demonstrates the usage of a do-while loop in JavaScript to print numbers from 1 to 10 and then from 100 onwards.

## Code Explanation

### Printing Numbers from 1 to 10

```javascript
let counter = 1
do {
    document.writeln(`<p>${counter}</p>`)
    counter++
} while (counter <= 10)
```

- `counter` is initialized to 1.
- The `do-while` loop executes the code block at least once and then repeats it as long as the condition `counter <= 10` remains true.
- Inside the loop, each iteration prints the current value of `counter` within a paragraph element.
- After printing, the `counter` is incremented by 1.

### Printing Numbers from 100 Onwards

```javascript
let counter2 = 100
do {
    document.writeln(`<p>${counter2}</p>`)
    counter2++
} while (counter2 <= 10)
```

- `counter2` is initialized to 100.
- Similarly, the `do-while` loop is used, but this time with a different condition, `counter2 <= 10`.
- However, this condition will always be false (`counter2` starts at 100 and increments indefinitely), so the loop will only execute once.
- It prints the value of `counter2`, which starts at 100, and then increments it.

## Conclusion

This example illustrates the basic syntax and behavior of a do-while loop in JavaScript. It is useful when you want to execute a block of code at least once, regardless of whether the condition is initially true or not, and then continue executing it as long as the condition remains true.
```
