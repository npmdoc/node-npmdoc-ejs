# npmdoc-ejs

#### api documentation for  [ejs (v2.5.6)](https://github.com/mde/ejs)  [![npm package](https://img.shields.io/npm/v/npmdoc-ejs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ejs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ejs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ejs)

#### Embedded JavaScript templates

[![NPM](https://nodei.co/npm/ejs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ejs)

- [https://npmdoc.github.io/node-npmdoc-ejs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ejs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ejs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ejs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ejs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ejs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matthew Eernisse",
        "url": "http://fleegix.org"
    },
    "bugs": {
        "url": "https://github.com/mde/ejs/issues"
    },
    "contributors": [
        {
            "name": "Timothy Gu",
            "url": "https://timothygu.github.io"
        }
    ],
    "dependencies": {},
    "description": "Embedded JavaScript templates",
    "devDependencies": {
        "browserify": "^13.0.1",
        "eslint": "^3.0.0",
        "git-directory-deploy": "^1.5.1",
        "istanbul": "~0.4.3",
        "jake": "^8.0.0",
        "jsdoc": "^3.4.0",
        "lru-cache": "^4.0.1",
        "mocha": "^3.0.2",
        "uglify-js": "^2.6.2"
    },
    "directories": {},
    "dist": {
        "shasum": "479636bfa3fe3b1debd52087f0acb204b4f19c88",
        "tarball": "https://registry.npmjs.org/ejs/-/ejs-2.5.6.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "homepage": "https://github.com/mde/ejs",
    "keywords": [
        "template",
        "engine",
        "ejs"
    ],
    "license": "Apache-2.0",
    "main": "./lib/ejs.js",
    "maintainers": [
        {
            "name": "mde"
        }
    ],
    "name": "ejs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/mde/ejs.git"
    },
    "scripts": {
        "coverage": "istanbul cover node_modules/mocha/bin/_mocha",
        "devdoc": "jake doc[dev]",
        "doc": "jake doc",
        "lint": "eslint \"**/*.js\" Jakefile",
        "test": "mocha"
    },
    "version": "2.5.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
