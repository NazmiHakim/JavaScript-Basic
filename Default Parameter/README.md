```markdown
# Default Parameter Example

This repository contains a simple example of using default parameters in JavaScript functions. The code demonstrates how to assign a default value to a function parameter and how it behaves when the parameter is not provided, explicitly set to `undefined`, or set to `null`.

## Code Explanation

The JavaScript function `register` takes two parameters: `name` and `gender`. The `gender` parameter has a default value of `"UNKNOWN"`. If `gender` is not provided or is `undefined`, it defaults to `"UNKNOWN"`.

```html
<head>
    <title>Default Parameter</title>
</head>
<script>
function register(name, gender = "UNKNOWN") {
    document.writeln(name, " ", gender, "<br>");
}

register("Nazmi", "Male");   // Outputs: Nazmi Male
register("Teramoz");         // Outputs: Teramoz UNKNOWN
register("Gatsu", undefined); // Outputs: Gatsu UNKNOWN
register("Gatsu", null);     // Outputs: Gatsu null
</script>
```

### Function Calls

1. **`register("Nazmi", "Male");`**:
   - This call provides both `name` and `gender`.
   - Output: `Nazmi Male`

2. **`register("Teramoz");`**:
   - This call provides only `name`, and `gender` defaults to `"UNKNOWN"`.
   - Output: `Teramoz UNKNOWN`

3. **`register("Gatsu", undefined);`**:
   - This call explicitly sets `gender` to `undefined`, so it defaults to `"UNKNOWN"`.
   - Output: `Gatsu UNKNOWN`

4. **`register("Gatsu", null);`**:
   - This call sets `gender` to `null`. Since `null` is a value, the default parameter is not used.
   - Output: `Gatsu null`
