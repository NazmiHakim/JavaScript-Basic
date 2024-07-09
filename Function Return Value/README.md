```markdown
# JavaScript Function Return Value Examples

This repository contains two HTML files demonstrating the use of JavaScript functions to return values and display them in the browser.

## Code 1: Function Return Value

This example defines a function `Hello` that takes two parameters, `firstName` and `lastName`, concatenates them into a greeting message, and returns the result. The returned value is then displayed on the webpage.

### HTML Code

```html
<!DOCTYPE html>
<html>
<head>
    <title>Function Return Value</title>
</head>
<body>
    <script>
        function Hello (firstName, lastName) {
            const say = `Hello ${firstName} ${lastName}`;
            return say;
        }

        const result = Hello("Nazmi", "Hakim");
        document.writeln(`<p>${result}</p>`);
    </script>
</body>
</html>
```

### How It Works

- The `Hello` function is defined to accept two arguments: `firstName` and `lastName`.
- Inside the function, a template literal is used to create a greeting message.
- The function returns the greeting message.
- The `Hello` function is called with the arguments "Nazmi" and "Hakim".
- The returned value is written to the document and displayed as a paragraph on the webpage.

## Code 2: Function Return Value with Conditional Logic

This example defines a function `Score` that takes a numeric value as input and returns a corresponding letter grade based on predefined ranges. The user's score is prompted, converted to a number, and then passed to the `Score` function. The result is displayed on the webpage.

### HTML Code

```html
<!DOCTYPE html>
<html>
<head>
    <title>Function Return Value2</title>
</head>
<body>
    <script>
        function Score(value) {
            if (value >= 90) {
                return "A";
            }
            if (value >= 80) {
                return "B";
            }
            if (value >= 70) {
                return "C";
            }
            if (value >= 60) {
                return "D";
            } else {
                return "E";
            }
        }

        const result = prompt("Enter your score:");
        const numericResult = Number(result);
        document.writeln(`<p>${Score(numericResult)}</p>`);
    </script>
</body>
</html>
```

### How It Works

- The `Score` function is defined to accept a numeric value as an argument.
- The function uses conditional logic to return a letter grade based on the value:
  - "A" for scores 90 and above.
  - "B" for scores 80 to 89.
  - "C" for scores 70 to 79.
  - "D" for scores 60 to 69.
  - "E" for scores below 60.
- The user is prompted to enter their score, which is then converted to a number.
- The numeric score is passed to the `Score` function.
- The returned grade is written to the document and displayed as a paragraph on the webpage.
