# @metaphorxyz/eslint-config
This package includes standard ESLint configurations for Metaphor projects.

## Usage
Install the package, and set it as the imported eslint config. The patch is necessary because of the way we handle dependencies relative to this project instead of requiring importing them all as peer dependencies on every Metaphor project.

```shell
> npm i --save-dev @metaphorxyz/eslint-config

or

> yarn add -D @metaphorxyz/eslint-config
```

```javascript
// .eslintrc.js
require("@metaphor-xyz/eslint-config/patch");

// Add your "extends" boilerplate here, for example:
module.exports = {
  extends: ['@metaphor-xyz/eslint-config'],
};
```

