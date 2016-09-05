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

First of all, you can use it, just like `cross-env`:

```
{
  "scripts": {
    "build": "run NODE_ENV=production webpack --config build/webpack.config.js"
  }
}

```

But you can use the same command directly from command line:

```
run NODE_ENV=production webpack --config build/webpack.config.js
```

You can put the same command as above to `script/build` and it cross-platform with:

```
run scripts/build
```

## LICENSE

MIT
