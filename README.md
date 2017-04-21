# npmtest-compose-middleware

#### basic test coverage for  [compose-middleware (v2.2.0)](https://github.com/blakeembrey/compose-middleware)  [![npm package](https://img.shields.io/npm/v/npmtest-compose-middleware.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-compose-middleware) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-compose-middleware.svg)](https://travis-ci.org/npmtest/node-npmtest-compose-middleware)

#### Compose an array of middleware into a single function for use in Express, Connect, router, etc.

[![NPM](https://nodei.co/npm/compose-middleware.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/compose-middleware)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-compose-middleware/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-compose-middleware/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-compose-middleware/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-compose-middleware/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-compose-middleware/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-compose-middleware/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-compose-middleware/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-compose-middleware/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-compose-middleware/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-compose-middleware/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-compose-middleware/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-compose-middleware/build/test-report.html](https://npmtest.github.io/node-npmtest-compose-middleware/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-compose-middleware/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-compose-middleware/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-compose-middleware/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-compose-middleware/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-compose-middleware/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-compose-middleware/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-compose-middleware/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-compose-middleware/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "compose-middleware",
    "version": "2.2.0",
    "description": "Compose an array of middleware into a single function for use in Express, Connect, router, etc.",
    "main": "lib/index.js",
    "typings": "lib/index.d.ts",
    "files": [
        "lib/",
        "LICENSE"
    ],
    "scripts": {
        "lint": "tslint \"src/**/*.ts\"",
        "build-ts": "tsc",
        "build": "rm -rf lib && npm run build-ts",
        "test-spec": "mocha lib/**/*.spec.js -R spec --bail",
        "test-cov": "istanbul cover -x *.spec.js node_modules/mocha/bin/_mocha -- lib/**/*.spec.js -R spec --bail",
        "test": "npm run build && npm run lint && npm run test-cov",
        "prepublish": "typings install && npm run build"
    },
    "repository": {
        "type": "git",
        "url": "git://github.com/blakeembrey/compose-middleware.git"
    },
    "keywords": [
        "middleware",
        "express",
        "compose",
        "flatten",
        "function"
    ],
    "author": {
        "name": "Blake Embrey",
        "url": "http://blakeembrey.me"
    },
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/blakeembrey/compose-middleware/issues"
    },
    "homepage": "https://github.com/blakeembrey/compose-middleware",
    "devDependencies": {
        "chai": "^3.2.0",
        "istanbul": "^0.4.4",
        "mocha": "^2.2.5",
        "tslint": "^3.11.0",
        "tslint-config-standard": "^1.2.2",
        "typescript": "^1.5.3",
        "typings": "^1.3.0"
    },
    "dependencies": {
        "array-flatten": "^2.1.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
