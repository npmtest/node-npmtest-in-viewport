# npmtest-in-viewport

#### basic test coverage for  [in-viewport (v3.4.2)](https://github.com/vvo/in-viewport#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-in-viewport.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-in-viewport) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-in-viewport.svg)](https://travis-ci.org/npmtest/node-npmtest-in-viewport)

#### Get a callback when an element enters the viewport (body) or a custom viewport

[![NPM](https://nodei.co/npm/in-viewport.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/in-viewport)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-in-viewport/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-in-viewport/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-in-viewport/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-in-viewport/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-in-viewport/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-in-viewport/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-in-viewport/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-in-viewport/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-in-viewport/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-in-viewport/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-in-viewport/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-in-viewport/build/test-report.html](https://npmtest.github.io/node-npmtest-in-viewport/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-in-viewport/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-in-viewport/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-in-viewport/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-in-viewport/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-in-viewport/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-in-viewport/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-in-viewport/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-in-viewport/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Vincent Voyer",
        "url": "http://github.com/vvo"
    },
    "bugs": {
        "url": "https://github.com/vvo/in-viewport/issues"
    },
    "dependencies": {},
    "description": "Get a callback when an element enters the viewport (body) or a custom viewport",
    "devDependencies": {
        "browserify": "^12.0.1",
        "closurecompiler": "^1.5.2",
        "deumdify": "^1.2.2",
        "merge": "1.2.0",
        "watchify": "^3.6.1",
        "zuul": "^3.11.0",
        "zuul-ngrok": "^4.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "400b1c759b4b305ef19249429b7f202cdc6b7427",
        "tarball": "https://registry.npmjs.org/in-viewport/-/in-viewport-3.4.2.tgz"
    },
    "gitHead": "b65a2c8def64b46ad1abe32880c724fc1849330c",
    "homepage": "https://github.com/vvo/in-viewport#readme",
    "license": "MIT",
    "main": "./in-viewport.js",
    "maintainers": [
        {
            "name": "tzi"
        },
        {
            "name": "vvo"
        }
    ],
    "name": "in-viewport",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/vvo/in-viewport.git"
    },
    "scripts": {
        "build": "browserify ./in-viewport.js -s inViewport -p deumdify | ccjs - > build/in-viewport.min.js",
        "dev": "npm run watch & DEBUG=zuul* zuul --local 8080 -- test/*.js",
        "test": "npm run build && DEBUG=zuul* zuul --tunnel ngrok -- test/*.js",
        "watch": "watchify ./in-viewport.js -d -s inViewport -p deumdify -o build/in-viewport.min.js -v"
    },
    "version": "3.4.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
