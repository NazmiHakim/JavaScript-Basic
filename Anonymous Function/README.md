```markdown
# Anonymous Function In Variable & Parameter

This project demonstrates the use of anonymous functions in JavaScript, both as variables and as parameters.

## Overview

The script includes examples of:
1. Assigning an anonymous function to a variable.
2. Passing an anonymous function as a parameter to another function.

## Code Explanation

### Declaring an Anonymous Function as a Variable

The following code assigns an anonymous function to the variable `say`:

```javascript
let say = function (name) {
    document.writeln(`Hello ${name}<br>`)
};

say("Nazmi");
```

This function takes a `name` parameter and writes a greeting to the document.

### Passing a Function as a Callback

The `giveMeName` function takes a callback function as a parameter and calls it with the argument `"Hakim"`:

```javascript
function giveMeName(callback) {
    callback("Hakim")
}

giveMeName(say);
```

Here, `giveMeName` is called with the `say` function as the callback, resulting in the output `Hello Hakim`.

### Using an Anonymous Function as a Callback

You can also pass an anonymous function directly as a parameter:

```javascript
giveMeName(function(name) {
    document.writeln(`<p>Hi ${name}</p>`);
});
```

This call results in the output `Hi Hakim` wrapped in a paragraph tag.

## Running the Script

To see the script in action:
1. Save the HTML and JavaScript code in a `.html` file.
2. Open the file in a web browser.

You should see the following output:

```
Hello Nazmi
Hello Hakim
Hi Hakim
```

## Conclusion

This example demonstrates how to use anonymous functions in JavaScript to create flexible and reusable code.
```

This README.md file provides an overview of the script, explains the code, and guides users on how to run the script.
