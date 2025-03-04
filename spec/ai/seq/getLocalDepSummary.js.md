# getLocalDepSummary.js

This module exports a single async function `getLocalDepSummary()` that returns a summary of local dependencies in the project.

## Function Signature

```javascript
async function getLocalDepSummary(): Promise<string>
```

## Description

The function reads the `package.json` file in the project root directory and extracts the local dependencies. It then returns a summary string containing the names and versions of the local dependencies.

## Usage

```javascript
const getLocalDepSummary = require('./getLocalDepSummary');

(async () => {
  const summary = await getLocalDepSummary();
  console.log(summary);
})();
```

## Dependencies

- `fs.promises`: Used to read the `package.json` file.

## Notes

- The function assumes that the `package.json` file is located in the project root directory.