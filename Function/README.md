```markdown
# JavaScript Hello World Functions

This project contains simple JavaScript functions that demonstrate how to print "Hello World" to the web page. 

## Description

The script defines two functions:
1. `sayHelloWorld()`: Prints "Hello World" once.
2. `sayHelloWorld10Times()`: Calls `sayHelloWorld()` 10 times to print "Hello World" ten times.

## Usage

Include the following HTML and JavaScript code in your project to use these functions.

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Function</title>
</head>
<body>
    <script src="script.js"></script>
</body>
</html>
```

### JavaScript (script.js)

```javascript
function sayHelloWorld() {
    document.writeln("Hello World", "<br>");
}

function sayHelloWorld10Times(){
    for (let i = 0; i < 10; i++) {
        sayHelloWorld(); 
    }
}

sayHelloWorld();
sayHelloWorld10Times();
```

## Output

When you open the `function.html` file in a browser, you should see "Hello World" printed eleven times on the web page.
