```markdown
# Optional Parameter Example

This example demonstrates how to use optional parameters in a JavaScript function. The function `Hello` is designed to accept three parameters: `firstName`, `midName`, and `lastName`. If fewer than three arguments are passed when calling the function, the missing arguments will be `undefined`.

## Usage

The `Hello` function logs the values of the parameters `firstName`, `midName`, and `lastName` to the console. It can be called with one, two, or three arguments.

## Code

```html
<head>
    <title>Optional Parameter</title>
</head>
<script>
    function Hello(firstName, midName, lastName) {
        console.log(firstName);
        console.log(midName);
        console.log(lastName);
    }

    Hello("Nazmi");
    // The midName and lastName will be shown as "undefined" in the console
    Hello("Nazmi", "Hakim", "Gatsu");
    Hello("Nazmi", "Hakim", "Gatsu", "Teramoz");
    // Teramoz will not be shown
</script>
```

## Explanation

- `Hello("Nazmi");`
  - Output:
    ```
    Nazmi
    undefined
    undefined
    ```

- `Hello("Nazmi", "Hakim", "Gatsu");`
  - Output:
    ```
    Nazmi
    Hakim
    Gatsu
    ```

- `Hello("Nazmi", "Hakim", "Gatsu", "Teramoz");`
  - Output:
    ```
    Nazmi
    Hakim
    Gatsu
    ```
  - The extra argument `Teramoz` is ignored since the function only accepts three parameters.

## Notes

- In JavaScript, when a function is called with fewer arguments than the function expects, the missing arguments are set to `undefined`.
- If a function is called with more arguments than it expects, the extra arguments are ignored.
- This example can be extended to handle optional parameters more gracefully using techniques like the rest operator or default values.
