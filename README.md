[![npm](https://img.shields.io/npm/v/@platypii/d3)](https://www.npmjs.com/package/@platypii/d3)
[![apache license](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)

# @types/d3

Standalone typescript definitions for [D3](https://github.com/d3/d3) javscript library.

## Why?

Because `@types/d3` depends on a bunch of sub-packages like `"@types/d3-array": "*"`.
I have a build system which doesn't like this, and would prefer version pegged dependencies.
So I made this package `@platypii/d3`.

## How to use

Add to `package.json`:
```json
{
  "devDependencies": {
    "@platypii/d3": "^0.0.1",
  }
}
```

Add to `tsconfig.json`:
```json
{
  "compilerOptions": {
    "typeRoots": [
      "node_modules/@types",
      "node_modules/@platypii"
    ]
  }
}
```

## Publishing

```
npm publish
```
