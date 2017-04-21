# npmdoc-jspdf

#### api documentation for  [jspdf (v1.3.3)](https://github.com/mrrio/jspdf)  [![npm package](https://img.shields.io/npm/v/npmdoc-jspdf.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jspdf) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jspdf.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jspdf)

#### PDF Document creation from JavaScript

[![NPM](https://nodei.co/npm/jspdf.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jspdf)

- [https://npmdoc.github.io/node-npmdoc-jspdf/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jspdf/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jspdf/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jspdf/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jspdf/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jspdf/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "jspdf",
    "version": "1.3.3",
    "homepage": "https://github.com/mrrio/jspdf",
    "description": "PDF Document creation from JavaScript",
    "main": "dist/jspdf.debug.js",
    "files": [
        "dist/jspdf.debug.js",
        "dist/jspdf.min.js",
        "README.md"
    ],
    "keywords": [
        "pdf"
    ],
    "license": "MIT",
    "repository": {
        "type": "git",
        "url": "https://github.com/MrRio/jsPDF.git"
    },
    "dependencies": {
        "adler32cs": "github:chick307/adler32cs.js",
        "cf-blob.js": "0.0.1",
        "filesaver.js": "github:andyinabox/FileSaver.js"
    },
    "devDependencies": {
        "babel-preset-es2015": "6.16.0",
        "babel-preset-es2015-rollup": "1.2.0",
        "codeclimate-test-reporter": "^0.4.0",
        "diff": "3.0.0",
        "docdash": "0.4.0",
        "jasmine": "2.5.2",
        "js-yaml": "3.6.1",
        "jsdoc": "3.4.2",
        "karma": "1.3.0",
        "karma-babel-preprocessor": "6.0.1",
        "karma-chrome-launcher": "2.0.0",
        "karma-coverage": "1.1.1",
        "karma-firefox-launcher": "1.0.0",
        "karma-jasmine": "1.0.2",
        "karma-mocha-reporter": "^2.2.0",
        "karma-sauce-launcher": "1.0.0",
        "local-web-server": "1.2.6",
        "markdown": "^0.5.0",
        "pdfjs-dist": "1.6.283",
        "rollup": "0.36.3",
        "rollup-plugin-babel": "2.6.1",
        "uglify-js": "2.7.3"
    },
    "scripts": {
        "start": "ws",
        "build": "npm install && bower install && node build.js",
        "version": "npm run build && git add -A dist",
        "test": "./node_modules/.bin/karma start saucelabs.karma.conf.js --single-run && for a in coverage/*; do codeclimate-test-reporter < \"$a/lcov.info\"; break; done",
        "test-local": "node tests/utils/reference-server.js & karma start",
        "generate-docs": "node_modules/.bin/jsdoc -c jsdoc.json --readme README.md"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
