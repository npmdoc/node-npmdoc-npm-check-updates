# npmdoc-npm-check-updates

#### basic api documentation for  [npm-check-updates (v2.11.0)](https://github.com/tjunnone/npm-check-updates)  [![npm package](https://img.shields.io/npm/v/npmdoc-npm-check-updates.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-npm-check-updates) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-npm-check-updates.svg)](https://travis-ci.org/npmdoc/node-npmdoc-npm-check-updates)

#### Find newer versions of dependencies than what your package.json or bower.json allows

[![NPM](https://nodei.co/npm/npm-check-updates.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/npm-check-updates)

- [https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tomas Junnonen"
    },
    "bin": {
        "npm-check-updates": "./bin/npm-check-updates",
        "ncu": "./bin/ncu"
    },
    "bugs": {
        "url": "https://github.com/tjunnone/npm-check-updates/issues"
    },
    "contributors": [
        {
            "name": "Raine Revere",
            "url": "https://github.com/raineorshine"
        }
    ],
    "dependencies": {
        "bluebird": "^3.4.3",
        "chalk": "^1.1.3",
        "cint": "^8.2.1",
        "cli-table": "^0.3.1",
        "commander": "^2.9.0",
        "fast-diff": "^1.0.1",
        "find-up": "1.1.2",
        "get-stdin": "^5.0.1",
        "json-parse-helpfulerror": "^1.0.3",
        "lodash": "^4.15.0",
        "node-alias": "^1.0.4",
        "npm": "^3.10.6",
        "npmi": "^2.0.1",
        "require-dir": "^0.3.0",
        "semver": "^5.3.0",
        "semver-utils": "^1.1.1",
        "snyk": "^1.25.1",
        "spawn-please": "^0.2.0",
        "update-notifier": "^1.0.2"
    },
    "description": "Find newer versions of dependencies than what your package.json or bower.json allows",
    "devDependencies": {
        "chai": "^3.5.0",
        "chai-as-promised": "^6.0.0",
        "chai-string": "^1.2.0",
        "chokidar-cli": "^1.2.0",
        "eslint": "^3.4.0",
        "mocha": "^3.0.2",
        "should": "^11.1.0",
        "tmp": "0.0.31"
    },
    "directories": {},
    "dist": {
        "shasum": "6073a2c022eaf27352e2a8b08de931776207b818",
        "tarball": "https://registry.npmjs.org/npm-check-updates/-/npm-check-updates-2.11.0.tgz"
    },
    "dynamicDependencies": {
        "bower": "^1.6.5"
    },
    "engines": {
        "node": ">=0.12"
    },
    "files": [
        "bin",
        "lib"
    ],
    "gitHead": "fe77ba1cd5705bc68b2e741eb76373b05c5d97d5",
    "homepage": "https://github.com/tjunnone/npm-check-updates",
    "keywords": [
        "npm",
        "bower",
        "check",
        "find",
        "discover",
        "updates",
        "upgrades",
        "dependencies",
        "package.json",
        "bower.json",
        "updater",
        "version",
        "management"
    ],
    "license": "Apache-2.0",
    "main": "./lib/npm-check-updates",
    "maintainers": [
        {
            "name": "tjunnone"
        },
        {
            "name": "raine"
        }
    ],
    "name": "npm-check-updates",
    "optionalDependencies": {},
    "preferGlobal": true,
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tjunnone/npm-check-updates.git"
    },
    "scripts": {
        "lint": "eslint bin lib test",
        "test": "npm run lint ; mocha && mocha test/individual",
        "watch": "chokidar \"lib/**/*.js\" -c \"npm run test\""
    },
    "version": "2.11.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
