# api documentation for  [sqs-consumer (v3.5.0)](https://github.com/BBC/sqs-consumer)  [![npm package](https://img.shields.io/npm/v/npmdoc-sqs-consumer.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-sqs-consumer) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sqs-consumer.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sqs-consumer)
#### Build SQS-based Node applications without the boilerplate

[![NPM](https://nodei.co/npm/sqs-consumer.png?downloads=true)](https://www.npmjs.com/package/sqs-consumer)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sqs-consumer/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-sqs-consumer%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sqs-consumer/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sqs-consumer/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sqs-consumer/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "robin@robinmurphy.co.uk"
    },
    "bugs": {
        "url": "https://github.com/BBC/sqs-consumer/issues"
    },
    "dependencies": {
        "async": "^2.0.1",
        "aws-sdk": "^2.0.23",
        "debug": "^2.1.0"
    },
    "description": "Build SQS-based Node applications without the boilerplate",
    "devDependencies": {
        "codeclimate-test-reporter": "0.4.1",
        "istanbul": "^0.4.1",
        "jshint": "^2.9.1",
        "mocha": "^3.0.2",
        "sinon": "^1.10.3"
    },
    "directories": {},
    "dist": {
        "shasum": "483b2c261ca5c9130489dafbacba3edb29f31a7f",
        "tarball": "https://registry.npmjs.org/sqs-consumer/-/sqs-consumer-3.5.0.tgz"
    },
    "gitHead": "1e195e542623d8aff531efaa2c28f419739fa438",
    "homepage": "https://github.com/BBC/sqs-consumer",
    "jshintConfig": {
        "quotmark": "single",
        "unused": true,
        "undef": true,
        "node": true,
        "globals": {
            "describe": false,
            "it": false,
            "before": false,
            "beforeEach": false,
            "after": false,
            "afterEach": false
        }
    },
    "keywords": [
        "sqs",
        "queue",
        "consumer"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "ibl",
            "email": "ibl-team@lists.forge.bbc.co.uk"
        }
    ],
    "name": "sqs-consumer",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/BBC/sqs-consumer.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha -- -R dot && open coverage/lcov-report/index.html",
        "lcov": "istanbul cover _mocha -- -R dot",
        "lint": "jshint .",
        "posttest": "npm run lint",
        "test": "mocha"
    },
    "version": "3.5.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module sqs-consumer](#apidoc.module.sqs-consumer)
1.  [function <span class="apidocSignatureSpan">sqs-consumer.</span>create (options)](#apidoc.element.sqs-consumer.create)
1.  [function <span class="apidocSignatureSpan">sqs-consumer.</span>super_ ()](#apidoc.element.sqs-consumer.super_)



# <a name="apidoc.module.sqs-consumer"></a>[module sqs-consumer](#apidoc.module.sqs-consumer)

#### <a name="apidoc.element.sqs-consumer.create"></a>[function <span class="apidocSignatureSpan">sqs-consumer.</span>create (options)](#apidoc.element.sqs-consumer.create)
- description and source-code
```javascript
create = function (options) {
  return new Consumer(options);
}
```
- example usage
```shell
...
'''

## Usage

'''js
const Consumer = require('sqs-consumer');

const app = Consumer.create({
  queueUrl: 'https://sqs.eu-west-1.amazonaws.com/account-id/queue-name',
  handleMessage: (message, done) => {
    // do some work with 'message'
    done();
  }
});
...
```

#### <a name="apidoc.element.sqs-consumer.super_"></a>[function <span class="apidocSignatureSpan">sqs-consumer.</span>super_ ()](#apidoc.element.sqs-consumer.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
