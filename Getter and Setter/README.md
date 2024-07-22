```markdown
# Getter and Setter in JavaScript

This repository demonstrates the use of getters and setters in JavaScript objects. The example provided is a simple implementation of a `person` object with `firstName` and `lastName` properties, as well as `fullName` getter and setter methods.

## Description

The script defines a `person` object with:
- `firstName`: Initial value is "Nazmi"
- `lastName`: Initial value is "Hakim"
- `fullName` getter: Returns the full name as a string.
- `fullName` setter: Logs a message to the document when the full name is changed.

## Usage

The example script demonstrates how to use the getter and setter methods. When the `fullName` property is set, it writes a message to the document. The `firstName` is then changed, and the `fullName` getter is used to write the updated full name to the document.

### Example Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Getter and Setter</title>
</head>
<body>
    <script>
        // Getter
        const person = {
            firstName: "Nazmi",
            lastName: "Hakim",
            get fullName() {
                return `${this.firstName} ${this.lastName} <br>`;
            },
            // Setter
            set fullName(value) {
                document.writeln(`Change Full Name ${value} <br>`);
            }
        };

        person.fullName = "Gatsu Berserk";

        person.firstName = "Teramoz";
        document.writeln(person.fullName);
    </script>
</body>
</html>
```

## Running the Example

1. Save the code above in an HTML file.
2. Open the file in a web browser.
3. Observe the changes in the document:
   - The message "Change Full Name Gatsu Berserk" will be displayed.
   - The full name "Teramoz Hakim" will be displayed.
