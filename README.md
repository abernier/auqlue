[![ci/cd](https://github.com/abernier/auqlue/workflows/ci/cd/badge.svg)](https://github.com/abernier/auqlue/actions?query=workflow%3Aci%2Fcd)
[![NPM version](https://img.shields.io/npm/v/auqlue.svg?style=flat)](https://www.npmjs.com/package/auqlue)

# AUQLUE

A sample repository published as a NPM package.

## Usage

```js
const answer = require('auqlue')

console.log('the Answer to the Ultimate Question of Life, the Universe, and Everything is:', answer)
```

## Publish to NPM

### Manually

1. bump the `package.json` version
2. 

### Using CI/CD

To release a new version on [npm](https://www.npmjs.com/package/auqlue):
1. bump the [`package.json` version](https://github.com/abernier/auqlue/edit/master/package.json)
2. then, create [a new realese](https://github.com/abernier/auqlue/releases/new) and wait for the [ci/cd](https://github.com/abernier/auqlue/actions?query=workflow%3Aci%2Fcd) publish it :)