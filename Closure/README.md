```markdown
# JavaScript Adder Function

This JavaScript code creates a function that adds a specified value to any given number and writes the result, along with the owner's name, to the document.

## How It Works

The script defines a function `createAdder` that takes a `value` as an argument. This function returns another function `add`, which takes a parameter `param`. The `add` function adds the `value` from the `createAdder` function to `param` and writes the owner's name to the document.

## Script Breakdown

1. **createAdder(value)**
    - This function takes a numerical value as an argument.
    - It sets a constant `owner` to the string "Eko".
    - It returns a nested function `add`.

2. **add(param)**
    - This nested function takes a numerical parameter `param`.
    - It writes the owner's name ("Eko") to the document.
    - It returns the sum of `value` and `param`.

3. **Using createAdder**
    - Two instances of the adder function are created with `const addTwo = createAdder(2);`.
    - The returned function `addTwo` is called with arguments 10 and 20.
    - The results are written to the document.

## Example

The script creates an adder function that adds 2 to any given number. When `addTwo(10)` is called, it writes "Eko" to the document and returns 12. Similarly, `addTwo(20)` writes "Eko" to the document and returns 22.

## Code

```html
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript Adder Function</title>
</head>
<body>
    <script>
        function createAdder(value) {
            const owner = "Eko";
            function add(param) {
                document.writeln(owner);
                return value + param;
            }
            return add;
        }  

        const addTwo = createAdder(2);
        document.writeln(addTwo(10));
        document.writeln(addTwo(20));
    </script>
</body>
</html>
```

## Usage

- Open the HTML file in a web browser.
- The browser will display the owner name "Eko" and the results of the addition operations.
