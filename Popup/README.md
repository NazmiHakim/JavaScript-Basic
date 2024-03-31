**README.md**

# Alert, Prompt, and Confirm

## Description

This repository contains examples of using JavaScript's `alert`, `prompt`, and `confirm` functions to interact with users via dialog boxes in web pages.

## Usage

### Alert

The `alert` function displays a message to the user in a dialog box with an "OK" button. It is commonly used to provide information or warnings.

#### Example:

```javascript
alert("This is a Warning");
```

### Prompt

The `prompt` function displays a dialog box with a message prompting the user to input text. It returns the text entered by the user as a string. 

#### Example:

```javascript
const name = prompt("Who is your name?");
alert(`Hello ${name}`);
```

### Confirm

The `confirm` function displays a dialog box with a message and two buttons: "OK" and "Cancel". It returns a boolean value (`true` if "OK" is clicked and `false` if "Cancel" is clicked).

#### Example:

```javascript
const enter = confirm("Do you want to enter?");
if (enter) {
    // Code to execute if the user clicks "OK"
    const name = prompt("Who is your name?");
    alert(`Hello ${name}`);
} else {
    // Code to execute if the user clicks "Cancel"
    alert("Bye bye");
}
```
