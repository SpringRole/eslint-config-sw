## Installation

Install the package with

```sh
npm install eslint-config-springworks --save-dev

# or
yarn add eslint-config-springworks -D
```

`eslint-config-springworks` requires you to take care of it's `peerDependencies`.
Install the correct version of each `peerDependencies` package, which are listed
with the following command:

```sh
npm info "eslint-config-springworks@latest" peerDependencies
```

If using npm 5+, use this shortcut:

```sh
npx install-peerdeps --dev eslint-config-springworks

# or
yarn add eslint-config-springworks -D --peer
```

## Usage

Now add `eslint-config-springworks` to either your `package.json`:

```json
{
  "eslintConfig": {
    "extends": "eslint-config-springworks"
  }
}
```

to your `.eslintrc`:

```json
{
  "extends": "eslint-config-springworks"
}
```

or `.eslintrc.js`:

```js
module.exports = {
  extends: 'eslint-config-springworks',
}
```

### Prettier Config

This is how you can use or extend the `eslint-config-springworks` prettier config in your
app:

```js
// prettier.config.js
module.exports = require('eslint-config-springworks/prettier.config')
```