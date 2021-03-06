## Installation

Install the package with

```sh
npm install eslint-config-sw-in-fe --save-dev

# or
yarn add eslint-config-sw-in-fe -D
```

`eslint-config-sw-in-fe` requires you to take care of it's `peerDependencies`.
Install the correct version of each `peerDependencies` package, which are listed
with the following command:

```sh
npm info "eslint-config-sw-in-fe@latest" peerDependencies
```

If using npm 5+, use this shortcut:

```sh
npx install-peerdeps --dev eslint-config-sw-in-fe

# or
yarn add eslint-config-sw-in-fe -D --peer
```

## Usage

Now add `eslint-config-sw-in-fe` to either your `package.json`:

```json
{
  "eslintConfig": {
    "extends": "eslint-config-sw-in-fe"
  }
}
```

to your `.eslintrc`:

```json
{
  "extends": "eslint-config-sw-in-fe"
}
```

or `.eslintrc.js`:

```js
module.exports = {
  extends: 'eslint-config-sw-in-fe'
};
```

### Prettier Config

This is how you can use or extend the `eslint-config-sw-in-fe` prettier config in your
app:

```js
// .prettierrc.js
module.exports = {
  ...require('eslint-config-sw-in-fe/prettier.config')
};
```
