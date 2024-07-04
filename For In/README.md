```markdown
# JavaScript Object Properties Example

This example demonstrates how to iterate over the properties of a JavaScript object using the `for...in` loop and display each property and its value on a webpage.

## HTML Structure

The HTML structure is minimal and includes a `<head>` section with a `<title>` tag:

```html
<head>
    <title>For In</title>
</head>
```

## JavaScript Code

The JavaScript code defines an object `person` with three properties: `firstName`, `midName`, and `lastName`. It then uses a `for...in` loop to iterate over the properties of the `person` object and writes each property and its value to the document:

```javascript
const person = {
    firstName: "Hakim",
    midName: "Teramoz",
    lastName: "Gatsu"
};

for (const property in person) {
    document.writeln(`<p> Property ${property} : ${person[property]}</p>`);
}
```

## Explanation

1. **Object Definition**:
    ```javascript
    const person = {
        firstName: "Hakim",
        midName: "Teramoz",
        lastName: "Gatsu"
    };
    ```
    An object `person` is defined with three properties: `firstName`, `midName`, and `lastName`.

2. **`for...in` Loop**:
    ```javascript
    for (const property in person) {
        document.writeln(`<p> Property ${property} : ${person[property]}</p>`);
    }
    ```
    The `for...in` loop iterates over all enumerable properties of the `person` object. For each property, it writes a paragraph (`<p>`) element to the document, displaying the property name and its corresponding value.

## Usage

To use this example, simply include the HTML and JavaScript code in an HTML file and open it in a web browser. The browser will display the properties and values of the `person` object as paragraphs on the webpage.

## Example Output

When the code is executed, the output on the webpage will be:

```
Property firstName : Hakim
Property midName : Teramoz
Property lastName : Gatsu
```

This output shows each property of the `person` object and its value.
