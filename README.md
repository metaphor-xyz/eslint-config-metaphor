# @metaphorxyz/eslint-config
This package includes standard ESLint configurations for Metaphor projects.

## Usage
Install the package, and set it as the imported eslint config. The patch is necessary because of the way we handle dependencies relative to this project instead of requiring importing them all as peer dependencies on every Metaphor project.

```shell
> npm i --save-dev @metaphorxyz/eslint-config @rushstack/eslint-patch

or

> yarn add -D @metaphorxyz/eslint-config @rushstack/eslint-patch
```

```javascript
// .eslintrc.js
require("@rushstack/eslint-patch/modern-module-resolution");

// Add your "extends" boilerplate here, for example:
module.exports = {
  extends: ['@metaphor-xyz/eslint-config'],
};
```

