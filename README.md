# test coverage for  [scripty (v1.7.1)](https://github.com/testdouble/scripty#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-scripty.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-scripty) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-scripty.svg)](https://travis-ci.org/npmtest/node-npmtest-scripty)
#### Because no one should be shell-scripting inside a JSON file.

[![NPM](https://nodei.co/npm/scripty.png?downloads=true)](https://www.npmjs.com/package/scripty)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-scripty/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-scripty/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-scripty/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-scripty/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-scripty/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-scripty/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-scripty/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-scripty/build/screenCapture.buildCustomOrg.browser.coverage.html.png)](https://npmtest.github.io/node-npmtest-scripty/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-scripty/build/screenCapture.buildCustomOrg.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmtest%252Fnode-npmtest-scripty%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-scripty/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-scripty/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-scripty%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-scripty/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-scripty/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-scripty/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Justin Searls",
        "email": "searls@gmail.com"
    },
    "bin": {
        "scripty": "cli.js"
    },
    "bugs": {
        "url": "https://github.com/testdouble/scripty/issues"
    },
    "dependencies": {
        "async": "^1.5.2",
        "glob": "^7.0.3",
        "lodash": "^4.8.2"
    },
    "description": "Because no one should be shell-scripting inside a JSON file.",
    "devDependencies": {
        "assert": "^1.3.0",
        "codeclimate-test-reporter": "^0.3.1",
        "intercept-stdout": "^0.1.2",
        "istanbul": "^0.4.3",
        "istanbul-combine": "github:searls/istanbul-combine",
        "semver": "^5.1.0",
        "standard": "^6.0.8",
        "teenytest": "^3.0.0",
        "testdouble": "^1.4.1"
    },
    "directories": {},
    "dist": {
        "shasum": "0ee86a2f333d2e4f6c14fabfb99d4cd6fc789bc5",
        "tarball": "https://registry.npmjs.org/scripty/-/scripty-1.7.1.tgz"
    },
    "gitHead": "b54fe4c6f689ab0e784a09da449e7b78f2df7478",
    "homepage": "https://github.com/testdouble/scripty#readme",
    "keywords": [
        "npm",
        "scripts",
        "dry",
        "scripts",
        "shell",
        "script",
        "management"
    ],
    "license": "MIT",
    "main": "lib/scripty.js",
    "maintainers": [
        {
            "name": "searls",
            "email": "searls@gmail.com"
        }
    ],
    "name": "scripty",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/testdouble/scripty.git"
    },
    "scripts": {
        "test": "npm run test:unit && npm run test:style && npm run test:safe",
        "test:cover": "npm run test:cover:unit && npm run test:cover:safe && npm run test:cover:combine",
        "test:cover:combine": "istanbul-combine -d coverage/combine coverage/unit/coverage.json coverage/safe/coverage.json",
        "test:cover:safe": "istanbul cover --dir coverage/safe teenytest -- \"test/safe/**/*.js\" --helper test/safe-helper.js",
        "test:cover:unit": "istanbul cover --dir coverage/unit teenytest -- \"lib/**/*.test.js\" --helper test/unit-helper.js",
        "test:cover:upload": "codeclimate-test-reporter < coverage/combine/lcov.info",
        "test:safe": "teenytest \"test/safe/**/*.js\" --helper test/safe-helper.js",
        "test:style": "standard",
        "test:unit": "teenytest \"lib/**/*.test.js\" --helper test/unit-helper.js"
    },
    "standard": {
        "globals": [
            "td",
            "assert",
            "UNSUPPORTED_TDD"
        ]
    },
    "version": "1.7.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
