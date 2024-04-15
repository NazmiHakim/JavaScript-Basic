```
# Optional Chaining

## Introduction
This is a simple demonstration of how to use optional chaining in JavaScript to access nested properties of objects without causing errors if any intermediate property is null or undefined.

## Code Explanation
In this example, we have a JavaScript object `person` representing a person with an optional `address` property. We want to access the `country` property nested within `address`.

### Without Optional Chaining
In traditional JavaScript syntax, we would access the `country` property like this:
```javascript
let country = person.address.country;
```
However, this approach could throw an error if `person`, `address`, or `country` is null or undefined.

### With Optional Chaining
Using optional chaining, we can access the `country` property safely:
```javascript
let country = person?.address?.country;
```
This syntax ensures that if `person`, `address`, or `country` is null or undefined, the `country` variable will be assigned `undefined` without causing an error.

## Output
The script outputs the value of `country` and a test message to the document.

## Additional Notes
Optional chaining (`?.`) is supported in modern JavaScript environments and provides a convenient way to handle potentially missing properties in nested objects.
```

Feel free to adjust the content as needed!
