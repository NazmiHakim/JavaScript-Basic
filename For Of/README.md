```markdown
# For Of Loop Example

This project demonstrates the use of the `for...of` loop in JavaScript to iterate over elements of an array and characters of a string, displaying the results in an HTML document.

## Files

### `index.html`

This file contains the HTML structure and the JavaScript code to perform the iteration and display the results.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Of</title>
</head>
<body>
    <script>
        const names = ["Nazmi", "Hakim"];
        for(const name of names) {
            document.writeln(`<p>${name}</p>`)
        }

        const fullname = "Nazmi Hakim"
        for(const character of fullname) {
            document.writeln(`<p>${character}</p>`)
        }
    </script>
</body>
</html>
```

### Description

- **Names Array Iteration**: The code iterates over an array of names (`names`), printing each name inside a `<p>` element.
- **Full Name String Iteration**: The code iterates over each character of a string (`fullname`), printing each character inside a `<p>` element.

### How to Use

1. Create an HTML file (e.g., `index.html`).
2. Copy and paste the provided HTML and JavaScript code into the file.
3. Open the HTML file in a web browser to see the output.

### Output

The output will display the following:
- Each name from the `names` array in a separate paragraph.
- Each character from the `fullname` string in a separate paragraph.

## Example

When you open the `index.html` file in a web browser, the output will look like this:

```
Nazmi
Hakim
N
a
z
m
i
 
H
a
k
i
m
```
