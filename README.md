# cross-run

Like [cross-env](https://github.com/kentcdodds/cross-env), but able to run npm scripts.

It prepends all npm paths like `node_modules/.bin` to `PATH` before executing provided script.

## Why?

Prepending npm binary paths to PATH allows shell-scripting outside of JSON file.

This package follows the mindset of [scripty](https://github.com/testdouble/scripty) but prefers to not use `npm run` at all.

## Installation

```
npm install -g cross-run
```

## Usage

1. **Remove** all non-lifecycle scripts from `package.json`

2. Create following script file in `scripts/build`:

```
cross-run NODE_ENV=production webpack --config build/webpack.config.js
```

3. You can run this script cross-platform with simple:

```
cross-run scripts/build
```

or even:

```
run scripts/build
```

## LICENSE

MIT
