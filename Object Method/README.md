```markdown
# Person Object Script

This script demonstrates the creation and usage of an object with methods in JavaScript. The `person` object has a method to greet and bid farewell to a person by their name.

## Usage

1. **Creating the `person` object**:
    The `person` object is created with an initial method `sayHello` to greet a person.

2. **Using the existing method**:
    The existing method `sayHello` is called with the argument `"Hakim"` to display an alert message.

3. **Adding a new method**:
    A new method `sayGoodbye` is added to the `person` object to bid farewell.

4. **Using the new method**:
    The new method `sayGoodbye` is called with the argument `"Hakim"` to display an alert message.

## Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Person Object Script</title>
</head>
<body>
    <script>
    // Making Object with Method
    const person = {
        name: "Nazmi",
        sayHello: function (name) {
            alert(`Hello ${name}, from ${this.name}`);
        }
    }
    
    // Existing method usage
    person.sayHello("Hakim");
    
    // Adding a new method to the object
    person.sayGoodbye = function(name) {
        alert(`Goodbye ${name}, from ${this.name}`);
    }
    
    // Using the new method
    person.sayGoodbye("Hakim");
    </script>
</body>
</html>
```

## Explanation

- **Creating the `person` object**:
  The `person` object is created with a property `name` and a method `sayHello` which takes a parameter `name` and displays an alert with a greeting message.

- **Using the existing method**:
  The method `sayHello` is called with the argument `"Hakim"`. The alert will display "Hello Hakim, from Nazmi".

- **Adding a new method**:
  A new method `sayGoodbye` is added to the `person` object, which also takes a parameter `name` and displays an alert with a farewell message.

- **Using the new method**:
  The method `sayGoodbye` is called with the argument `"Hakim"`. The alert will display "Goodbye Hakim, from Nazmi".

## Conclusion

This script provides a simple example of creating an object with methods in JavaScript, using existing methods, and dynamically adding new methods to the object.
