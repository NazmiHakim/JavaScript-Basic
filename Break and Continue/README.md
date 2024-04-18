
```
# JavaScript Break & Continue

This JavaScript code demonstrates the use of the `break` and `continue` statements within loops.

## Break Statement

The `break` statement is used to terminate the loop it is in. In the provided code, it is used within a `while` loop to break out of the loop when the `counter` variable exceeds 10.

### Code Explanation:

```javascript
let counter = 1;
while (true) {
    document.writeln(`<p>${counter}</p>`); // Display the current value of counter
    counter++; // Increment counter

    if (counter > 10) {
        break; // Exit the loop if counter exceeds 10
    }
}

## Continue Statement

The `continue` statement is used to skip the current iteration of a loop and proceed to the next iteration. In the provided code, it is used within a `for` loop to skip even numbers and continue with the next iteration.

### Code Explanation:

```javascript
for(let i = 1; i <= 100; i++) {
    if (i % 2 === 0) { // Check if the current number is even
        continue; // Skip the current iteration if it's even
    }
    document.writeln(`<p>${i}</p>`); // Display the current odd number
}
```

## How to Run:

To run this code, simply embed it within an HTML file and open it in a web browser.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Break & Continue</title>
</head>
<body>
    <script>
        // Place the JavaScript code here
    </script>
</body>
</html>
```

This README provides an overview of how the `break` and `continue` statements work in JavaScript loops and how they are implemented in the provided code.
```
