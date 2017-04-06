# api documentation for  [express-ipfilter (v0.2.3)](https://github.com/baminteractive/express-ipfilter#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-express-ipfilter.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-express-ipfilter) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-express-ipfilter.svg)](https://travis-ci.org/npmdoc/node-npmdoc-express-ipfilter)
#### A light-weight IP address based filtering system

[![NPM](https://nodei.co/npm/express-ipfilter.png?downloads=true)](https://www.npmjs.com/package/express-ipfilter)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-ipfilter/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-express-ipfilter_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-ipfilter/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-express-ipfilter/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-express-ipfilter/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "BaM Interactive"
    },
    "bugs": {
        "url": "https://github.com/baminteractive/express-ipfilter/issues"
    },
    "dependencies": {
        "ip": "~1.1.0",
        "lodash": "~3.10.1",
        "range_check": "^1.2.0"
    },
    "description": "A light-weight IP address based filtering system",
    "devDependencies": {
        "babel-preset-es2015": "^6.6.0",
        "grunt": "^0.4.5",
        "grunt-babel": "^6.0.0",
        "grunt-check-dependencies": "^0.12.0",
        "grunt-cli": "^1.2.0",
        "grunt-contrib-copy": "^0.8.2",
        "grunt-contrib-watch": "^0.6.1",
        "grunt-eslint": "^19.0.0",
        "grunt-mocha-istanbul": "^3.0.1",
        "grunt-mocha-test": "~0.12.7",
        "istanbul": "^0.4.0",
        "load-grunt-tasks": "^3.3.0",
        "minimatch": "^3.0.3",
        "mocha": "^2.5.3",
        "mocha-junit-reporter": "^1.9.1",
        "publish": "^0.5.0"
    },
    "directories": {},
    "dist": {
        "shasum": "c22603b5027b92a2ea8f3797aceaa4833bfdb42d",
        "tarball": "https://registry.npmjs.org/express-ipfilter/-/express-ipfilter-0.2.3.tgz"
    },
    "homepage": "https://github.com/baminteractive/express-ipfilter#readme",
    "keywords": [
        "middleware",
        "ipfilter",
        "ip filter",
        "ipban",
        "ip ban",
        "express"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "ryanbillingsley",
            "email": "ryanbbillingsley@gmail.com"
        }
    ],
    "name": "express-ipfilter",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/baminteractive/express-ipfilter.git"
    },
    "scripts": {
        "push": "publish",
        "test": "mocha -R spec"
    },
    "version": "0.2.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module express-ipfilter](#apidoc.module.express-ipfilter)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.</span>IpDeniedError (message, extra)](#apidoc.element.express-ipfilter.IpDeniedError)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.</span>IpDeniedError.super_ ()](#apidoc.element.express-ipfilter.IpDeniedError.super_)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.</span>IpFilter (ips, opts)](#apidoc.element.express-ipfilter.IpFilter)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.</span>deniedError (message, extra)](#apidoc.element.express-ipfilter.deniedError)

#### [module express-ipfilter.IpDeniedError](#apidoc.module.express-ipfilter.IpDeniedError)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.</span>IpDeniedError (message, extra)](#apidoc.element.express-ipfilter.IpDeniedError.IpDeniedError)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.IpDeniedError.</span>super_ ()](#apidoc.element.express-ipfilter.IpDeniedError.super_)

#### [module express-ipfilter.IpDeniedError.super_](#apidoc.module.express-ipfilter.IpDeniedError.super_)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.IpDeniedError.</span>super_ ()](#apidoc.element.express-ipfilter.IpDeniedError.super_.super_)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.IpDeniedError.super_.</span>captureStackTrace ()](#apidoc.element.express-ipfilter.IpDeniedError.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">express-ipfilter.IpDeniedError.super_.</span>stackTraceLimit

#### [module express-ipfilter.deniedError](#apidoc.module.express-ipfilter.deniedError)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.</span>deniedError (message, extra)](#apidoc.element.express-ipfilter.deniedError.deniedError)
1.  [function <span class="apidocSignatureSpan">express-ipfilter.deniedError.</span>super_ ()](#apidoc.element.express-ipfilter.deniedError.super_)



# <a name="apidoc.module.express-ipfilter"></a>[module express-ipfilter](#apidoc.module.express-ipfilter)

#### <a name="apidoc.element.express-ipfilter.IpDeniedError"></a>[function <span class="apidocSignatureSpan">express-ipfilter.</span>IpDeniedError (message, extra)](#apidoc.element.express-ipfilter.IpDeniedError)
- description and source-code
```javascript
function IpDeniedError(message, extra) {
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message || 'The requesting IP was denied';
  this.extra = extra;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-ipfilter.IpDeniedError.super_"></a>[function <span class="apidocSignatureSpan">express-ipfilter.</span>IpDeniedError.super_ ()](#apidoc.element.express-ipfilter.IpDeniedError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-ipfilter.IpFilter"></a>[function <span class="apidocSignatureSpan">express-ipfilter.</span>IpFilter (ips, opts)](#apidoc.element.express-ipfilter.IpFilter)
- description and source-code
```javascript
function ipfilter(ips, opts) {
  ips = ips || false;

  var logger = function logger(message) {
    console.log(message);
  };
  var settings = _.defaults(opts || {}, {
    mode: 'deny',
    log: true,
    logF: logger,
    allowedHeaders: [],
    allowPrivateIPs: false,
    excluding: [],
    detectIp: getClientIp
  });

  function getClientIp(req) {
    var ipAddress;

    var headerIp = _.reduce(settings.allowedHeaders, function (acc, header) {
      var testIp = req.headers[header];
      if (testIp != '') {
        acc = testIp;
      }

      return acc;
    }, '');

    if (headerIp) {
      var splitHeaderIp = headerIp.split(',');
      ipAddress = splitHeaderIp[0];
    }

    if (!ipAddress) {
      ipAddress = req.connection.remoteAddress;
    }

    if (!ipAddress) {
      return '';
    }

    if (iputil.isV6Format(ipAddress) && ~ipAddress.indexOf('::ffff')) {
      ipAddress = ipAddress.split('::ffff:')[1];
    }

    return ipAddress;
  }

  var matchClientIp = function matchClientIp(ip) {
    var mode = settings.mode.toLowerCase();

    var result = _.invoke(ips, testIp, ip, mode);

    if (mode === 'allow') {
      return _.some(result);
    } else {
      return _.every(result);
    }
  };

  var testIp = function testIp(ip, mode) {
    var constraint = this;

    // Check if it is an array or a string
    if (typeof constraint === 'string') {
      if (rangeCheck.validRange(constraint)) {
        return testCidrBlock(ip, constraint, mode);
      } else {
        return testExplicitIp(ip, constraint, mode);
      }
    }

    if ((typeof constraint === 'undefined' ? 'undefined' : _typeof(constraint)) === 'object') {
      return testRange(ip, constraint, mode);
    }
  };

  var testExplicitIp = function testExplicitIp(ip, constraint, mode) {
    if (ip === constraint) {
      return mode === 'allow';
    } else {
      return mode === 'deny';
    }
  };

  var testCidrBlock = function testCidrBlock(ip, constraint, mode) {
    if (rangeCheck.inRange(ip, constraint)) {
      return mode === 'allow';
    } else {
      return mode === 'deny';
    }
  };

  var testRange = function testRange(ip, constraint, mode) {
    var filteredSet = _.filter(ips, function (constraint) {
      if (constraint.length > 1) {
        var startIp = iputil.toLong(constraint[0]);
        var endIp = iputil.toLong(constraint[1]);
        var longIp = iputil.toLong(ip);
        return longIp >= startIp && longIp <= endIp;
      } else {
        return ip === constraint[0];
      }
    });

    if (filteredSet.length > 0) {
      return mode === 'allow';
    } else {
      return mode === 'deny';
    }
  };

  return function (req, res, next) {
    if (settings.excluding.length > 0) {
      var results = _.filter(settings.excluding, function (exclude) {
        var regex = new RegExp(exclude);
        return regex.test(req.url);
      });

      if (results.length > 0) {
        if (settings.log && settings.logLevel !== 'deny') {
          settings.logF('Access granted for excluded path: ' + results[0]);
        }
        return next();
      }
    }

    var ip = settings.detectIp(req);
    // If no IPs were specified, skip
    // this middleware
    if (!ips || !ips.length) {
      return next();
    }

    if (matchClientIp(ip, req)) {
      // Grant access
      if (settings.log && settings.logLevel !== 'deny') {
        settings.logF('Access granted to IP address: ' + ip);
      }

      return next();
    }

    // Deny access
    if (settings.log && settings.logLevel !== 'allow') {
      settings.logF('Access denied to IP address: ' + ip);
    }

    var err = new IpDeniedError('Access denied to IP address: ' + ip);
    return next(err);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-ipfilter.deniedError"></a>[function <span class="apidocSignatureSpan">express-ipfilter.</span>deniedError (message, extra)](#apidoc.element.express-ipfilter.deniedError)
- description and source-code
```javascript
function IpDeniedError(message, extra) {
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message || 'The requesting IP was denied';
  this.extra = extra;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-ipfilter.IpDeniedError"></a>[module express-ipfilter.IpDeniedError](#apidoc.module.express-ipfilter.IpDeniedError)

#### <a name="apidoc.element.express-ipfilter.IpDeniedError.IpDeniedError"></a>[function <span class="apidocSignatureSpan">express-ipfilter.</span>IpDeniedError (message, extra)](#apidoc.element.express-ipfilter.IpDeniedError.IpDeniedError)
- description and source-code
```javascript
function IpDeniedError(message, extra) {
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message || 'The requesting IP was denied';
  this.extra = extra;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-ipfilter.IpDeniedError.super_"></a>[function <span class="apidocSignatureSpan">express-ipfilter.IpDeniedError.</span>super_ ()](#apidoc.element.express-ipfilter.IpDeniedError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-ipfilter.IpDeniedError.super_"></a>[module express-ipfilter.IpDeniedError.super_](#apidoc.module.express-ipfilter.IpDeniedError.super_)

#### <a name="apidoc.element.express-ipfilter.IpDeniedError.super_.super_"></a>[function <span class="apidocSignatureSpan">express-ipfilter.IpDeniedError.</span>super_ ()](#apidoc.element.express-ipfilter.IpDeniedError.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-ipfilter.IpDeniedError.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">express-ipfilter.IpDeniedError.super_.</span>captureStackTrace ()](#apidoc.element.express-ipfilter.IpDeniedError.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
...






module.exports = function IpDeniedError(message, extra) {
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message || 'The requesting IP was denied';
  this.extra = extra;
};

require('util').inherits(module.exports, Error);
...
```



# <a name="apidoc.module.express-ipfilter.deniedError"></a>[module express-ipfilter.deniedError](#apidoc.module.express-ipfilter.deniedError)

#### <a name="apidoc.element.express-ipfilter.deniedError.deniedError"></a>[function <span class="apidocSignatureSpan">express-ipfilter.</span>deniedError (message, extra)](#apidoc.element.express-ipfilter.deniedError.deniedError)
- description and source-code
```javascript
function IpDeniedError(message, extra) {
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message || 'The requesting IP was denied';
  this.extra = extra;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-ipfilter.deniedError.super_"></a>[function <span class="apidocSignatureSpan">express-ipfilter.deniedError.</span>super_ ()](#apidoc.element.express-ipfilter.deniedError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
