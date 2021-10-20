## prettier
### Install:

```bash
yarn add @caisy/prettier -D
```

### Usage:

Use one of the tree approaches:
1. Add it to your package.json:

```json
{
  "prettier": "@caisy/prettier"
}
```
2. Add it to your .prettierrc.json:

"@caisy/prettier"

3. If you want to override some properties of the config:
```js
// .prettierrc.js
module.exports = {
  ...require('@caisy/prettier'),
  semi: false,
};
```

### Ignoring Code:
1. Use this, if you do not want to extend the .prettierignore:
```bash
npx prettier ** --write --ignore-path node_modules/@caisy/prettier/.prettierignore
```