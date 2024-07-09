```markdown
# Function Return Value Example

This project demonstrates a simple JavaScript function that returns a greeting message and displays it on an HTML page.

## Description

The HTML file contains a JavaScript function `Hello` which takes two arguments, `firstName` and `lastName`, and returns a greeting message. The result of the function is then written to the HTML document.

## Files

- `index.html`: Contains the HTML structure and the JavaScript function.

## Usage

To run this example, simply open the `index.html` file in a web browser. The greeting message will be displayed on the page.

## Code Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Function Return Value</title>
</head>
<body>
    <script>
        function Hello(firstName, lastName) {
            const say = `Hello ${firstName} ${lastName}`;
            return say;
        }

        const result = Hello("Nazmi", "Hakim");
        document.writeln(`<p>${result}</p>`);
    </script>
</body>
</html>
```

## How It Works

1. The `Hello` function takes two parameters: `firstName` and `lastName`.
2. It constructs a greeting message using template literals.
3. The function returns the greeting message.
4. The returned value is assigned to the `result` variable.
5. The `result` is written to the HTML document using `document.writeln`.
