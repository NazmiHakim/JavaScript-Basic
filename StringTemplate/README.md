# JavaScript String Template

This repository contains JavaScript code demonstrating the usage of string templates, variable insertion, expressions within templates, and multiline strings.

## Usage

### 1. String Templates

The script utilizes string templates to dynamically generate strings by embedding variables and expressions within backticks (\`\`). 

```javascript
const name = "Nazmi Hakim";
const firstName = "Nazmi";
const lastName = "Hakim";
const value = 80;

const template = `Name : ${name} <br> ${firstName} ${lastName} <br>`;
console.info(template);
document.writeln(template);
```

### 2. Expressions in String Templates

Expressions can be used within string templates. In this case, a boolean expression checks if the value is greater than 75.

```javascript
const template2 = `Name : ${name} <br> Pass : ${value > 75} <br>`;
document.writeln(template2);
```

### 3. Multiline Strings

Multiline strings can be created using backticks. This maintains the formatting of the string.

```javascript
let multilinestring = `Name : Nazmi Hakim
NIM : 2310817210012 
Gender : Male 
Height : 182cm 
Weight : 66kg
`;
document.writeln("<pre>");
document.writeln(multilinestring);
document.writeln("<pre>");
```
