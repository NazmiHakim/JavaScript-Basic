```markdown
# With Statement Example

This project demonstrates the usage of the `with` statement in JavaScript to simplify the access of properties within an object.

## Files

### `index.html`

This file contains the HTML structure and the JavaScript code to demonstrate the usage of the `with` statement.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>With Statement</title>
</head>
<body>
    <script>
        // Without "With Statement"
        const person = {
            firstName: "Hakim",
            midName: "Teramoz",
            lastName: "Gatsu"
        }

        console.log(person.firstName);
        console.log(person.midName);
        console.log(person.lastName);

        // With "With Statement"
        with (person) {
            console.log(firstName);
            console.log(midName);
            console.log(lastName);
        }
    </script>
</body>
</html>
```

### Description

- **Without `with` Statement**: The code accesses and logs each property of the `person` object individually using `person.propertyName`.
- **With `with` Statement**: The code accesses and logs the properties of the `person` object using the `with` statement, which allows for a simpler syntax.

### How to Use

1. Create an HTML file (e.g., `index.html`).
2. Copy and paste the provided HTML and JavaScript code into the file.
3. Open the HTML file in a web browser and check the console output.

### Output

The console will display the following output:

```
Hakim
Teramoz
Gatsu
Hakim
Teramoz
Gatsu
```

### Explanation

- **Without `with` Statement**:
  - Each property of the `person` object is accessed and logged individually.
- **With `with` Statement**:
  - The `with` statement is used to access the properties of the `person` object directly, simplifying the code.

### Note

The `with` statement is generally discouraged in modern JavaScript due to potential confusion and conflicts in scope resolution. It is included here for educational purposes to demonstrate its usage and behavior.
