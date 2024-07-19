---

# Recursive Function Script

## Description

This script demonstrates the calculation of the factorial of a number using both iterative and recursive approaches. The results of the calculations are then displayed on the webpage.

## Contents

1. **Iterative Factorial Calculation**: Uses a loop to calculate the factorial.
2. **Recursive Factorial Calculation**: Uses a recursive function to calculate the factorial.

## Usage

To use this script, simply include it in an HTML file and open the file in a web browser. The script will automatically calculate and display the factorials.

### Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recursive Function</title>
</head>
<body>
    <script>
        // Factorial loop
        function factorial(value) {
            let result = 1;
            for (let i = 1; i <= value; i++) {
                result *= i;
            }
            return result;
        }

        document.writeln(factorial(5), "<br>");
        document.writeln(1 * 2 * 3 * 4 * 5, "<br>");

        // Factorial recursive
        function factorialRecursive(value) {
            if (value === 1) {
                return 1;
            } else {
                return value * factorialRecursive(value - 1);
            }
        }

        document.writeln(factorialRecursive(7), "<br>");
        document.writeln(1 * 2 * 3 * 4 * 5 * 6 * 7);
    </script>
</body>
</html>
```

## Explanation

- **Iterative Factorial Calculation**:
    - The function `factorial(value)` initializes a variable `result` to 1.
    - It then loops from 1 to the input `value`, multiplying `result` by each number in the sequence.
    - The final result is returned and written to the document.

- **Recursive Factorial Calculation**:
    - The function `factorialRecursive(value)` checks if the input `value` is 1.
    - If it is, the function returns 1.
    - Otherwise, it returns `value` multiplied by the result of calling `factorialRecursive` with `value - 1`.
    - The final result is written to the document.

This script effectively demonstrates both approaches to calculating the factorial of a number.

---
