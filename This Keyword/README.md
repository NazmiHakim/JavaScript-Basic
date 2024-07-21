```markdown
# Console Log This

This project demonstrates the use of `this` in different scopes within JavaScript. It logs the value of `this` in the global scope, within a function, and within an object method.

## Files

- `index.html`: The main HTML file containing the script.

## Usage

1. Open `index.html` in a web browser.
2. Open the browser's developer console to view the output of the `console.info` statements.
3. Observe how the value of `this` changes in different contexts.

## Code Explanation

### Global Scope

```javascript
console.info(this);
```

In the global scope, `this` refers to the global object, which is `window` in browsers.

### Function Scope

```javascript
function sample() {
    console.info(this);

    function sample2() {
        console.info(this);
    }

    sample2();
}

sample();
```

Within the `sample` function, `this` also refers to the global object because `sample` is a regular function call. The same applies to the `sample2` function nested within `sample`.

### Object Method

```javascript
const person = {
    name: "Hakim",
    sayHello: function (name) {
        // this = person
        document.write(`Hi ${name}, my name is ${this.name}`)
    }
}

person.sayHello("Teramoz");
```

Within the `sayHello` method of the `person` object, `this` refers to the `person` object itself. This allows access to the object's properties, such as `name`.

## License

This project is open source and available under the MIT License.
