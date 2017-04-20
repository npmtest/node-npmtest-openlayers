# npmtest-openlayers

#### basic test coverage for  [openlayers (v4.1.0)](https://openlayers.org/)  [![npm package](https://img.shields.io/npm/v/npmtest-openlayers.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-openlayers) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-openlayers.svg)](https://travis-ci.org/npmtest/node-npmtest-openlayers)

#### Build tools and sources for developing OpenLayers based mapping applications

[![NPM](https://nodei.co/npm/openlayers.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/openlayers)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-openlayers/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-openlayers/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-openlayers/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-openlayers/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-openlayers/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-openlayers/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-openlayers/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-openlayers/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-openlayers/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-openlayers/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-openlayers/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-openlayers/build/test-report.html](https://npmtest.github.io/node-npmtest-openlayers/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-openlayers/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-openlayers/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-openlayers/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-openlayers/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-openlayers/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-openlayers/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-openlayers/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-openlayers/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "browser": "dist/ol.js",
    "bugs": {
        "url": "https://github.com/openlayers/openlayers/issues"
    },
    "dependencies": {
        "async": "2.3.0",
        "browserify": "14.3.0",
        "closure-util": "1.18.0",
        "derequire": "2.0.6",
        "fs-extra": "2.1.2",
        "glob": "7.1.1",
        "handlebars": "4.0.6",
        "jsdoc": "3.4.3",
        "marked": "0.3.6",
        "metalsmith": "2.3.0",
        "metalsmith-layouts": "1.8.0",
        "nomnom": "1.8.1",
        "pbf": "3.0.5",
        "pixelworks": "1.1.0",
        "rbush": "2.0.1",
        "temp": "0.8.3",
        "vector-tile": "1.3.0",
        "walk": "2.3.9"
    },
    "description": "Build tools and sources for developing OpenLayers based mapping applications",
    "devDependencies": {
        "clean-css-cli": "4.0.12",
        "coveralls": "2.13.0",
        "debounce": "^1.0.0",
        "eslint": "3.18.0",
        "eslint-config-openlayers": "7.0.0",
        "eslint-plugin-openlayers-internal": "^3.1.0",
        "expect.js": "0.3.1",
        "gaze": "^1.0.0",
        "istanbul": "0.4.5",
        "jquery": "3.2.1",
        "jscodeshift": "^0.3.30",
        "mocha": "3.2.0",
        "mocha-phantomjs-core": "^2.1.0",
        "mustache": "2.3.0",
        "phantomjs-prebuilt": "2.1.14",
        "proj4": "2.4.3",
        "resemblejs": "2.2.3",
        "serve-files": "1.0.1",
        "sinon": "2.1.0",
        "slimerjs": "0.10.3"
    },
    "directories": {},
    "dist": {
        "shasum": "22c4fa237aa3c596b6e81305eaaf570a2cb0e4ac",
        "tarball": "https://registry.npmjs.org/openlayers/-/openlayers-4.1.0.tgz"
    },
    "eslintConfig": {
        "extends": "openlayers",
        "globals": {
            "ArrayBuffer": false,
            "Float32Array": false,
            "Uint16Array": false,
            "Uint32Array": false,
            "Uint8Array": false,
            "Uint8ClampedArray": false,
            "ol": false,
            "goog": false,
            "proj4": false
        },
        "plugins": [
            "openlayers-internal"
        ],
        "rules": {
            "no-constant-condition": 0,
            "openlayers-internal/enum": 2,
            "openlayers-internal/no-duplicate-requires": 2,
            "openlayers-internal/no-missing-requires": 1,
            "openlayers-internal/no-unused-requires": 2,
            "openlayers-internal/one-provide": 2,
            "openlayers-internal/requires-first": 2,
            "openlayers-internal/valid-provide": 2,
            "openlayers-internal/valid-requires": 2
        }
    },
    "ext": [
        {
            "module": "rbush",
            "browserify": true
        },
        {
            "module": "pbf",
            "browserify": true
        },
        {
            "module": "pixelworks",
            "browserify": true
        },
        {
            "module": "vector-tile",
            "name": "vectortile",
            "browserify": true
        }
    ],
    "gitHead": "2b5d6536cafc3449ac50df0e5edf126d998baff5",
    "homepage": "https://openlayers.org/",
    "keywords": [
        "map",
        "mapping",
        "ol"
    ],
    "license": "BSD-2-Clause",
    "main": "dist/ol.js",
    "maintainers": [
        {
            "name": "ahocevar"
        },
        {
            "name": "bartvde"
        },
        {
            "name": "elemoine"
        },
        {
            "name": "fredj"
        },
        {
            "name": "marcjansen"
        },
        {
            "name": "tschaub"
        }
    ],
    "name": "openlayers",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/openlayers/openlayers.git"
    },
    "scripts": {
        "debug-server": "node tasks/serve-lib.js",
        "install": "node tasks/install.js",
        "postinstall": "closure-util update",
        "pretest": "eslint tasks test test_rendering src examples",
        "start": "node tasks/serve.js",
        "test": "node tasks/test.js"
    },
    "style": [
        "css/ol.css"
    ],
    "version": "4.1.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
