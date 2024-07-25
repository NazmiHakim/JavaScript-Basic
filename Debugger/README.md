```markdown
# Debugger Example

## Description

This project contains a simple JavaScript function to demonstrate debugging using the `debugger` statement. The function `createFullName` constructs a full name from given first, middle, and last names, but includes a deliberate mistake for debugging purposes.

## Files

- `index.html`: Contains the HTML structure and the embedded JavaScript code.

## Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Debugger</title>
</head>
<body>
<script>
function createFullName(firstName, middleName, lastName){
    debugger;
    const fullName = `${firstName} ${lastName} ${lastName}`; // Deliberate mistake for debugging
    return fullName;
}

createFullName("Nazmi", "Teramoz", "Hakim");
</script>
</body>
</html>
```

## Purpose

The purpose of this project is to:
1. Demonstrate the use of the `debugger` statement in JavaScript.
2. Illustrate how to step through code execution using browser developer tools.
3. Identify and fix a deliberate mistake in the code.

## Instructions

1. Open `index.html` in a web browser.
2. Open the browser's developer tools (usually by pressing `F12` or `Ctrl+Shift+I`).
3. Navigate to the "Sources" tab.
4. Reload the page and notice that the code execution pauses at the `debugger` statement.
5. Step through the code to inspect the values of variables and identify the deliberate mistake.
6. Fix the mistake in the code:
   ```javascript
   const fullName = `${firstName} ${middleName} ${lastName}`;
   ```
7. Verify the corrected code by running it again.

## Expected Output

After fixing the mistake, the function `createFullName("Nazmi", "Teramoz", "Hakim")` should return:

```
"Nazmi Teramoz Hakim"
```
