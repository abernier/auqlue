[![ci/cd](https://github.com/abernier/auqlue/workflows/ci/cd/badge.svg)](https://github.com/abernier/auqlue/actions?query=workflow%3Aci%2Fcd)
[![NPM version](https://img.shields.io/npm/v/auqlue.svg?style=flat)](https://www.npmjs.com/package/auqlue)

A sample repository published as a NPM package.

# Usage

```js
const answer = require('auqlue')

console.log('the Answer to the Ultimate Question of Life, the Universe, and Everything is:', answer)
```

# Publish to NPM

## Manually

1. bump the `package.json` version
2. `npm login` if not already
3. `npm publish`

If successful, you should want to tag the version:
```shell
$ git add package.json
$ git commit -m "bump version"
$ git tag v1.0.1
$ git push --tags
```

## Using [CI/CD](https://github.com/abernier/auqlue/actions?query=workflow%3Aci%2Fcd) workflow

Pre-requisite:
1. Generate a NPM token
2. Set it as `NPM_TOKEN` secret (as referenced into [`cicd.yml`](https://github.com/abernier/auqlue/blob/master/.github/workflows/cicd.yml#L37) file)

Then, to release a new version on [npm](https://www.npmjs.com/package/auqlue):
1. bump the [`package.json` version](https://github.com/abernier/auqlue/edit/master/package.json)
2. then, create [a new realese](https://github.com/abernier/auqlue/releases/new) and wait for the [ci/cd](https://github.com/abernier/auqlue/actions?query=workflow%3Aci%2Fcd) publish it :)
   ![](https://assets.codepen.io/67030/release.png)
