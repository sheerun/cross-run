![cross-run](https://i.imgur.com/wy8KYEE.png)

[![Unix CI](https://img.shields.io/travis/sheerun/cross-run/master.svg)](https://travis-ci.org/sheerun/cross-run)
[![Modern Node](https://img.shields.io/badge/modern-node-9BB48F.svg)](https://github.com/sheerun/modern-node)

**[DEPRECATED]** [cross-env](https://www.npmjs.com/package/cross-env) now supports npm scripts, please use it instead

> Like [cross-env](https://github.com/kentcdodds/cross-env), but able to run npm scripts.

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

```json
{
  "scripts": {
    "build": "run NODE_ENV=production webpack --config build/webpack.config.js"
  }
}

```

But you can use the same command directly from command line:

```sh
run NODE_ENV=production webpack --config build/webpack.config.js
```

You can put the same command as above to `script/build` and it cross-platform with:

```sh
run scripts/build
```

## LICENSE

MIT
# https://tea.xyz/what-is-this-file
---
version: 1.0.0
codeOwners:
  - '0x9a83D81E53a3a284Ae7EDC06Ede2B51a9523f2BF'
quorum: 1

