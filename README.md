# npmdoc-is_js

#### api documentation for  [is_js (v0.9.0)](http://is.js.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-is_js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-is_js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-is_js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-is_js)

#### micro check library

[![NPM](https://nodei.co/npm/is_js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/is_js)

- [https://npmdoc.github.io/node-npmdoc-is_js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-is_js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-is_js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-is_js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-is_js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-is_js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/arasatasaygin/is.js/issues"
    },
    "dependencies": {},
    "description": "micro check library",
    "devDependencies": {
        "chai": "^3.4.0",
        "eslint": "^2.13.1",
        "lodash": "^4.15.0",
        "mocha": "^2.2.1",
        "mocha-phantomjs": "^4.1.0",
        "pre-commit": "^1.1.3",
        "uglify-js": "^2.7.3"
    },
    "directories": {},
    "dist": {
        "shasum": "0ab94540502ba7afa24c856aa985561669e9c52d",
        "tarball": "https://registry.npmjs.org/is_js/-/is_js-0.9.0.tgz"
    },
    "files": [
        "is.js",
        "is.min.js"
    ],
    "homepage": "http://is.js.org/",
    "license": "MIT",
    "main": "is.js",
    "maintainers": [
        {
            "name": "arasatasaygin"
        },
        {
            "name": "jdalton"
        }
    ],
    "name": "is_js",
    "optionalDependencies": {},
    "pre-commit": [
        "lint"
    ],
    "repository": {
        "type": "git",
        "url": "git+https://github.com/arasatasaygin/is.js.git"
    },
    "scripts": {
        "build": "npm run lint && npm run min",
        "lint": "eslint .",
        "min": "uglifyjs is.js -m --comments \"/^!/\" -o is.min.js",
        "test": "mocha --check-leaks -R dot",
        "test:phantom": "mocha-phantomjs -R dot test/index.html"
    },
    "version": "0.9.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
