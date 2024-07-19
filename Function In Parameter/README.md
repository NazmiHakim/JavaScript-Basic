```markdown
# Function In Parameter

This project demonstrates the usage of functions as parameters in JavaScript. It covers how functions can be assigned to variables, passed as arguments, and invoked using callbacks.

## Code Explanation

### HTML Structure

The HTML structure includes a simple `<head>` section with a title:

```html
<head>
<title>Function In Parameter</title>
</head>
```

### JavaScript Code

The JavaScript code demonstrates several key concepts:

1. **Function Declaration and Invocation:**

   The `sayHello` function is declared to accept a `name` parameter and output a greeting:

   ```javascript
   function sayHello(name) {
       document.writeln(`<p>Hello ${name}</p>`)
   }

   // Invoke the function
   sayHello("Nazmi");
   ```

   When `sayHello("Nazmi")` is called, it writes "Hello Nazmi" to the document.

2. **Assigning Function to a Variable:**

   The `sayHello` function is assigned to a new variable `say`:

   ```javascript
   const say = sayHello;

   // Invoke the function using the new variable
   say("Hakim");
   ```

   Invoking `say("Hakim")` outputs "Hello Hakim" to the document.

3. **Passing Function as a Callback:**

   The `giveMeName` function accepts a callback function and invokes it with a given name:

   ```javascript
   function giveMeName(callback) {
       callback("Teramoz");
   }

   // Pass `sayHello` as a callback
   giveMeName(sayHello);
   ```

   When `giveMeName(sayHello)` is called, it invokes `sayHello("Teramoz")`, writing "Hello Teramoz" to the document.

### Full Code

```html
<head>
<title>Function In Parameter</title>
</head>
<script>
function sayHello(name){
    document.writeln(`<p>Hello ${name}</p>`)
}

sayHello("Nazmi")

const say = sayHello;

say("Hakim");

function giveMeName(callback){
    callback("Teramoz")
}

giveMeName(sayHello);
</script>
```

## How to Run

1. Copy the full code into an HTML file (e.g., `index.html`).
2. Open the HTML file in a web browser.
3. The browser will display three greetings:
   - "Hello Nazmi"
   - "Hello Hakim"
   - "Hello Teramoz"

## Concepts Covered

- Function declaration and invocation
- Assigning functions to variables
- Passing functions as arguments (callbacks)
```

This `README.md` provides an overview of the code, explaining the functionality and how to run it.
