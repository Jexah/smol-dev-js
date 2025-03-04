# extractJsonArray.js

This module exports a function `extractJsonArray` that takes a string as input and returns an array of JSON objects.

## Usage

```javascript
const extractJsonArray = require('./extractJsonArray');

const input = '[{"key1": "value1"}, {"key2": "value2"}]';
const output = extractJsonArray(input);

console.log(output); // [{key1: "value1"}, {key2: "value2"}]
```

## Function: extractJsonArray(input)

- **input**: `string` - A string containing a JSON array.

- **returns**: `Array` - An array of JSON objects extracted from the input string.

### Description

The `extractJsonArray` function takes a string as input and attempts to parse it as a JSON array. If the input is a valid JSON array, the function returns an array of JSON objects. If the input is not a valid JSON array, the function returns an empty array.

## Error Handling

If the input string is not a valid JSON array, the function will return an empty array.