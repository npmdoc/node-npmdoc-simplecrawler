# npmdoc-simplecrawler

#### api documentation for  [simplecrawler (v1.1.1)](https://github.com/cgiffard/node-simplecrawler)  [![npm package](https://img.shields.io/npm/v/npmdoc-simplecrawler.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-simplecrawler) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-simplecrawler.svg)](https://travis-ci.org/npmdoc/node-npmdoc-simplecrawler)

#### Very straightforward, event driven web crawler. Features a flexible queue interface and a basic cache mechanism with extensible backend.

[![NPM](https://nodei.co/npm/simplecrawler.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/simplecrawler)

- [https://npmdoc.github.io/node-npmdoc-simplecrawler/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christopher Giffard"
    },
    "bin": {
        "crawl": "./lib/cli.js"
    },
    "bugs": {
        "url": "https://github.com/cgiffard/node-simplecrawler/issues"
    },
    "dependencies": {
        "async": "^2.1.4",
        "iconv-lite": "^0.4.13",
        "robots-parser": "^1.0.0",
        "urijs": "^1.16.1"
    },
    "description": "Very straightforward, event driven web crawler. Features a flexible queue interface and a basic cache mechanism with extensible backend.",
    "devDependencies": {
        "chai": "^3.2.0",
        "eslint": "^2.0.0",
        "jsdoc": "^3.4.0",
        "mocha": "^3.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "5893d24d25ca67ca1244d813ff56ca04fadbdbe9",
        "tarball": "https://registry.npmjs.org/simplecrawler/-/simplecrawler-1.1.1.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "files": [
        "lib"
    ],
    "gitHead": "28aee5dc5d9123efb6ab4314cea4d0b7a3a25b59",
    "homepage": "https://github.com/cgiffard/node-simplecrawler",
    "keywords": [
        "simple",
        "crawler",
        "spider",
        "cache",
        "queue",
        "simplecrawler",
        "eventemitter"
    ],
    "license": "BSD-2-Clause",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "cgiffard"
        },
        {
            "name": "fredrikekelund"
        }
    ],
    "name": "simplecrawler",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/cgiffard/node-simplecrawler.git"
    },
    "scripts": {
        "docs": "jsdoc -c jsdoc.json",
        "lint": "eslint example/ lib/ test/",
        "mocha": "mocha -R spec -t 5000",
        "test": "npm run lint && npm run mocha"
    },
    "version": "1.1.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
