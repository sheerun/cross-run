# npm-env

Like [cross-env](https://github.com/kentcdodds/cross-env) but using [execa](https://github.com/sindresorhus/execa)

## Why?

As execa prepends npm binary paths to PATH, it allows shell-scripting outside of JSON file.

## Installation

```
npm install -g npm-env
```

## Usage

1. **Remove** all non-lifecycle scripts from `package.json`

2. Create following script file in `scripts/build`:

```
npm-env NODE_ENV=production webpack --config build/webpack.config.js
```

3. You can run this script cross-platform with simple:

```
npm-env scripts/build
```

## LICENSE

MIT
