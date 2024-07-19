```markdown
# Function In Function Example

This repository contains a simple JavaScript example demonstrating the concept of nested functions.

## Code Explanation

### JavaScript Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Function In Function</title>
</head>
<body>
    <script>
        function outer() {
            console.info("Outer");
            
            function inner() {
                console.info("Inner");
            }

            inner();
            inner();
        }

        outer();
        inner(); // ERROR: inner is not defined
    </script>
</body>
</html>
```

### Description

- **outer function**: 
  - This function logs "Outer" to the console.
  - It contains a nested function called `inner`.
  - The `inner` function logs "Inner" to the console.
  - The `inner` function is called twice within the `outer` function.

- **inner function**:
  - Defined within the `outer` function.
  - Only accessible within the scope of the `outer` function.
  - Calling `inner` inside `outer` works as expected.
  - Calling `inner` outside the `outer` function results in an error (`inner is not defined`).

### Running the Code

1. Open the `index.html` file in a web browser.
2. Open the browser's developer console (usually accessible via F12 or right-click > Inspect).
3. Observe the console output:
    - "Outer" followed by "Inner" twice.
    - An error message indicating that `inner` is not defined outside of `outer`.

### Key Points

- **Scope**: Functions defined within another function are only accessible within the outer function's scope.
- **Error Handling**: Attempting to call an inner function outside of its defining scope results in a reference error.

## Conclusion

This example demonstrates how function scope works in JavaScript, specifically highlighting the limitations of accessing nested functions from outside their parent functions.

## Additional Notes

- Make sure to include an `index.html` file with the provided HTML and JavaScript code.
- If distributing this repository, consider adding a `LICENSE` file for proper licensing.

## Contact

For any questions or issues, please contact the repository owner.
