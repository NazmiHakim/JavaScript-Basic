```markdown
# Function As Value

This is a simple HTML and JavaScript example demonstrating how functions can be assigned to variables and called using those variables.

## Description

The HTML file contains a script that defines a function `sayHello(name)`, which writes a greeting message to the document. The function is then assigned to a variable `say`, and both the original function and the variable are used to call the function with different arguments.

## Code

```html
<!DOCTYPE html>
<html>
<head>
    <title>Function As Value</title>
</head>
<body>
<script>
function sayHello(name){
    document.writeln(`Hello ${name} <br>`)
}

let say = sayHello;

sayHello("Nazmi");
say("Hakim");
</script>
</body>
</html>
```

## How to Use

1. Save the above code in an HTML file (e.g., `index.html`).
2. Open the HTML file in a web browser.
3. You will see two lines of output:
    ```
    Hello Nazmi 
    Hello Hakim 
    ```

## Explanation

- `sayHello(name)`: A function that takes a `name` parameter and writes a greeting message to the document.
- `let say = sayHello;`: The `sayHello` function is assigned to the variable `say`.
- `sayHello("Nazmi");`: Calls the `sayHello` function with the argument "Nazmi".
- `say("Hakim");`: Calls the `sayHello` function through the variable `say` with the argument "Hakim".

This example demonstrates that in JavaScript, functions can be assigned to variables and can be called using these variables, providing flexibility in how functions are used.
