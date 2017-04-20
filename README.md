# npmdoc-blessed

#### api documentation for  [blessed (v0.1.81)](https://github.com/chjj/blessed)  [![npm package](https://img.shields.io/npm/v/npmdoc-blessed.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-blessed) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-blessed.svg)](https://travis-ci.org/npmdoc/node-npmdoc-blessed)

#### A high-level terminal interface library for node.js.

[![NPM](https://nodei.co/npm/blessed.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/blessed)

- [https://npmdoc.github.io/node-npmdoc-blessed/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-blessed/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-blessed/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-blessed/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-blessed/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-blessed/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "blessed",
    "description": "A high-level terminal interface library for node.js.",
    "author": "Christopher Jeffrey",
    "version": "0.1.81",
    "license": "MIT",
    "main": "./lib/blessed.js",
    "bin": "./bin/tput.js",
    "preferGlobal": false,
    "repository": "git://github.com/chjj/blessed.git",
    "homepage": "https://github.com/chjj/blessed",
    "bugs": {
        "url": "http://github.com/chjj/blessed/issues"
    },
    "keywords": [
        "curses",
        "tui",
        "tput",
        "terminfo",
        "termcap"
    ],
    "tags": [
        "curses",
        "tui",
        "tput",
        "terminfo",
        "termcap"
    ],
    "engines": {
        "node": ">= 0.8.0"
    },
    "browserify": {
        "transform": [
            "./browser/transform.js"
        ]
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
