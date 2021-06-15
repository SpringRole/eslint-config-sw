## Installation

Install the package with

```sh
npm install eslint-config-sw-in --save-dev

# or
yarn add eslint-config-sw-in -D
```

`eslint-config-sw-in` requires you to take care of it's `peerDependencies`.
Install the correct version of each `peerDependencies` package, which are listed
with the following command:

```sh
npm info "eslint-config-sw-in@latest" peerDependencies
```

If using npm 5+, use this shortcut:

```sh
npx install-peerdeps --dev eslint-config-sw-in

# or
yarn add eslint-config-sw-in -D --peer
```

## Usage

Now add `eslint-config-sw-in` to either your `package.json`:

```json
{
  "eslintConfig": {
    "extends": "eslint-config-sw-in"
  }
}
```

to your `.eslintrc`:

```json
{
  "extends": "eslint-config-sw-in"
}
```

or `.eslintrc.js`:

```js
module.exports = {
  extends: 'eslint-config-sw-in',
}
```

### Prettier Config

This is how you can use or extend the `eslint-config-sw-in` prettier config in your
app:

```js
// prettier.config.js
module.exports = require('eslint-config-sw-in/prettier.config')
```