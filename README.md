# api documentation for  [passport (v0.3.2)](http://passportjs.org/)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-passport.svg)](https://travis-ci.org/npmdoc/node-npmdoc-passport)
#### Simple, unobtrusive authentication for Node.js.

[![NPM](https://nodei.co/npm/passport.png?downloads=true)](https://www.npmjs.com/package/passport)

[![apidoc](https://npmdoc.github.io/node-npmdoc-passport/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-passport_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-passport/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-passport/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Jared Hanson",
        "email": "jaredhanson@gmail.com",
        "url": "http://www.jaredhanson.net/"
    },
    "bugs": {
        "url": "http://github.com/jaredhanson/passport/issues"
    },
    "dependencies": {
        "passport-strategy": "1.x.x",
        "pause": "0.0.1"
    },
    "description": "Simple, unobtrusive authentication for Node.js.",
    "devDependencies": {
        "chai": "2.x.x",
        "chai-connect-middleware": "0.3.x",
        "chai-passport-strategy": "0.2.x",
        "mocha": "2.x.x",
        "proxyquire": "1.x.x"
    },
    "directories": {},
    "dist": {
        "shasum": "9dd009f915e8fe095b0124a01b8f82da07510102",
        "tarball": "https://registry.npmjs.org/passport/-/passport-0.3.2.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "gitHead": "ee57813037914642906aa9ed9e1c9ecbebf905ff",
    "homepage": "http://passportjs.org/",
    "keywords": [
        "express",
        "connect",
        "auth",
        "authn",
        "authentication"
    ],
    "license": "MIT",
    "licenses": [
        {
            "type": "MIT",
            "url": "http://www.opensource.org/licenses/MIT"
        }
    ],
    "main": "./lib",
    "maintainers": [
        {
            "name": "jaredhanson",
            "email": "jaredhanson@gmail.com"
        }
    ],
    "name": "passport",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jaredhanson/passport.git"
    },
    "scripts": {
        "test": "mocha --reporter spec --require test/bootstrap/node test/*.test.js test/**/*.test.js"
    },
    "version": "0.3.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module passport](#apidoc.module.passport)
1.  [function <span class="apidocSignatureSpan">passport.</span>Authenticator ()](#apidoc.element.passport.Authenticator)
1.  [function <span class="apidocSignatureSpan">passport.</span>Passport ()](#apidoc.element.passport.Passport)
1.  [function <span class="apidocSignatureSpan">passport.</span>Strategy ()](#apidoc.element.passport.Strategy)
1.  [function <span class="apidocSignatureSpan">passport.</span>strategies.SessionStrategy ()](#apidoc.element.passport.strategies.SessionStrategy)
1.  object <span class="apidocSignatureSpan">passport.</span>Authenticator.prototype
1.  object <span class="apidocSignatureSpan">passport.</span>Strategy.prototype
1.  object <span class="apidocSignatureSpan">passport.</span>_deserializers
1.  object <span class="apidocSignatureSpan">passport.</span>_framework
1.  object <span class="apidocSignatureSpan">passport.</span>_infoTransformers
1.  object <span class="apidocSignatureSpan">passport.</span>_serializers
1.  object <span class="apidocSignatureSpan">passport.</span>_strategies
1.  object <span class="apidocSignatureSpan">passport.</span>strategies
1.  object <span class="apidocSignatureSpan">passport.</span>strategies.SessionStrategy.prototype
1.  string <span class="apidocSignatureSpan">passport.</span>_key
1.  string <span class="apidocSignatureSpan">passport.</span>_userProperty

#### [module passport.Authenticator](#apidoc.module.passport.Authenticator)
1.  [function <span class="apidocSignatureSpan">passport.</span>Authenticator ()](#apidoc.element.passport.Authenticator.Authenticator)

#### [module passport.Authenticator.prototype](#apidoc.module.passport.Authenticator.prototype)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>_strategy (name)](#apidoc.element.passport.Authenticator.prototype._strategy)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>authenticate (strategy, options, callback)](#apidoc.element.passport.Authenticator.prototype.authenticate)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>authorize (strategy, options, callback)](#apidoc.element.passport.Authenticator.prototype.authorize)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>deserializeUser (fn, req, done)](#apidoc.element.passport.Authenticator.prototype.deserializeUser)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>framework (fw)](#apidoc.element.passport.Authenticator.prototype.framework)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>init ()](#apidoc.element.passport.Authenticator.prototype.init)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>initialize (options)](#apidoc.element.passport.Authenticator.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>serializeUser (fn, req, done)](#apidoc.element.passport.Authenticator.prototype.serializeUser)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>session (options)](#apidoc.element.passport.Authenticator.prototype.session)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>transformAuthInfo (fn, req, done)](#apidoc.element.passport.Authenticator.prototype.transformAuthInfo)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>unuse (name)](#apidoc.element.passport.Authenticator.prototype.unuse)
1.  [function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>use (name, strategy)](#apidoc.element.passport.Authenticator.prototype.use)

#### [module passport.Strategy](#apidoc.module.passport.Strategy)
1.  [function <span class="apidocSignatureSpan">passport.</span>Strategy ()](#apidoc.element.passport.Strategy.Strategy)

#### [module passport.Strategy.prototype](#apidoc.module.passport.Strategy.prototype)
1.  [function <span class="apidocSignatureSpan">passport.Strategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport.Strategy.prototype.authenticate)

#### [module passport._framework](#apidoc.module.passport._framework)
1.  [function <span class="apidocSignatureSpan">passport._framework.</span>authenticate (passport, name, options, callback)](#apidoc.element.passport._framework.authenticate)
1.  [function <span class="apidocSignatureSpan">passport._framework.</span>initialize (passport)](#apidoc.element.passport._framework.initialize)

#### [module passport.strategies](#apidoc.module.passport.strategies)
1.  [function <span class="apidocSignatureSpan">passport.strategies.</span>SessionStrategy ()](#apidoc.element.passport.strategies.SessionStrategy)

#### [module passport.strategies.SessionStrategy](#apidoc.module.passport.strategies.SessionStrategy)
1.  [function <span class="apidocSignatureSpan">passport.strategies.</span>SessionStrategy ()](#apidoc.element.passport.strategies.SessionStrategy.SessionStrategy)
1.  [function <span class="apidocSignatureSpan">passport.strategies.SessionStrategy.</span>super_ ()](#apidoc.element.passport.strategies.SessionStrategy.super_)

#### [module passport.strategies.SessionStrategy.prototype](#apidoc.module.passport.strategies.SessionStrategy.prototype)
1.  [function <span class="apidocSignatureSpan">passport.strategies.SessionStrategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport.strategies.SessionStrategy.prototype.authenticate)



# <a name="apidoc.module.passport"></a>[module passport](#apidoc.module.passport)

#### <a name="apidoc.element.passport.Authenticator"></a>[function <span class="apidocSignatureSpan">passport.</span>Authenticator ()](#apidoc.element.passport.Authenticator)
- description and source-code
```javascript
function Authenticator() {
  this._key = 'passport';
  this._strategies = {};
  this._serializers = [];
  this._deserializers = [];
  this._infoTransformers = [];
  this._framework = null;
  this._userProperty = 'user';

  this.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Passport"></a>[function <span class="apidocSignatureSpan">passport.</span>Passport ()](#apidoc.element.passport.Passport)
- description and source-code
```javascript
function Authenticator() {
  this._key = 'passport';
  this._strategies = {};
  this._serializers = [];
  this._deserializers = [];
  this._infoTransformers = [];
  this._framework = null;
  this._userProperty = 'user';

  this.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Strategy"></a>[function <span class="apidocSignatureSpan">passport.</span>Strategy ()](#apidoc.element.passport.Strategy)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.strategies.SessionStrategy"></a>[function <span class="apidocSignatureSpan">passport.</span>strategies.SessionStrategy ()](#apidoc.element.passport.strategies.SessionStrategy)
- description and source-code
```javascript
function SessionStrategy() {
  Strategy.call(this);
  this.name = 'session';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport.Authenticator"></a>[module passport.Authenticator](#apidoc.module.passport.Authenticator)

#### <a name="apidoc.element.passport.Authenticator.Authenticator"></a>[function <span class="apidocSignatureSpan">passport.</span>Authenticator ()](#apidoc.element.passport.Authenticator.Authenticator)
- description and source-code
```javascript
function Authenticator() {
  this._key = 'passport';
  this._strategies = {};
  this._serializers = [];
  this._deserializers = [];
  this._infoTransformers = [];
  this._framework = null;
  this._userProperty = 'user';

  this.init();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport.Authenticator.prototype"></a>[module passport.Authenticator.prototype](#apidoc.module.passport.Authenticator.prototype)

#### <a name="apidoc.element.passport.Authenticator.prototype._strategy"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>_strategy (name)](#apidoc.element.passport.Authenticator.prototype._strategy)
- description and source-code
```javascript
_strategy = function (name) {
  return this._strategies[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>authenticate (strategy, options, callback)](#apidoc.element.passport.Authenticator.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (strategy, options, callback) {
  return this._framework.authenticate(this, strategy, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.authorize"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>authorize (strategy, options, callback)](#apidoc.element.passport.Authenticator.prototype.authorize)
- description and source-code
```javascript
authorize = function (strategy, options, callback) {
  options = options || {};
  options.assignProperty = 'account';

  var fn = this._framework.authorize || this._framework.authenticate;
  return fn(this, strategy, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.deserializeUser"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>deserializeUser (fn, req, done)](#apidoc.element.passport.Authenticator.prototype.deserializeUser)
- description and source-code
```javascript
deserializeUser = function (fn, req, done) {
  if (typeof fn === 'function') {
    return this._deserializers.push(fn);
  }

  // private implementation that traverses the chain of deserializers,
  // attempting to deserialize a user
  var obj = fn;

  // For backwards compatibility
  if (typeof req === 'function') {
    done = req;
    req = undefined;
  }

  var stack = this._deserializers;
  (function pass(i, err, user) {
    // deserializers use 'pass' as an error to skip processing
    if ('pass' === err) {
      err = undefined;
    }
    // an error or deserialized user was obtained, done
    if (err || user) { return done(err, user); }
    // a valid user existed when establishing the session, but that user has
    // since been removed
    if (user === null || user === false) { return done(null, false); }

    var layer = stack[i];
    if (!layer) {
      return done(new Error('Failed to deserialize user out of session'));
    }


    function deserialized(e, u) {
      pass(i + 1, e, u);
    }

    try {
      var arity = layer.length;
      if (arity == 3) {
        layer(req, obj, deserialized);
      } else {
        layer(obj, deserialized);
      }
    } catch(e) {
      return done(e);
    }
  })(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.framework"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>framework (fw)](#apidoc.element.passport.Authenticator.prototype.framework)
- description and source-code
```javascript
framework = function (fw) {
  this._framework = fw;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.init"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>init ()](#apidoc.element.passport.Authenticator.prototype.init)
- description and source-code
```javascript
init = function () {
  this.framework(require('./framework/connect')());
  this.use(new SessionStrategy());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.initialize"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>initialize (options)](#apidoc.element.passport.Authenticator.prototype.initialize)
- description and source-code
```javascript
initialize = function (options) {
  options = options || {};
  this._userProperty = options.userProperty || 'user';

  return this._framework.initialize(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.serializeUser"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>serializeUser (fn, req, done)](#apidoc.element.passport.Authenticator.prototype.serializeUser)
- description and source-code
```javascript
serializeUser = function (fn, req, done) {
  if (typeof fn === 'function') {
    return this._serializers.push(fn);
  }

  // private implementation that traverses the chain of serializers, attempting
  // to serialize a user
  var user = fn;

  // For backwards compatibility
  if (typeof req === 'function') {
    done = req;
    req = undefined;
  }

  var stack = this._serializers;
  (function pass(i, err, obj) {
    // serializers use 'pass' as an error to skip processing
    if ('pass' === err) {
      err = undefined;
    }
    // an error or serialized object was obtained, done
    if (err || obj || obj === 0) { return done(err, obj); }

    var layer = stack[i];
    if (!layer) {
      return done(new Error('Failed to serialize user into session'));
    }


    function serialized(e, o) {
      pass(i + 1, e, o);
    }

    try {
      var arity = layer.length;
      if (arity == 3) {
        layer(req, user, serialized);
      } else {
        layer(user, serialized);
      }
    } catch(e) {
      return done(e);
    }
  })(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.session"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>session (options)](#apidoc.element.passport.Authenticator.prototype.session)
- description and source-code
```javascript
session = function (options) {
  return this.authenticate('session', options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.transformAuthInfo"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>transformAuthInfo (fn, req, done)](#apidoc.element.passport.Authenticator.prototype.transformAuthInfo)
- description and source-code
```javascript
transformAuthInfo = function (fn, req, done) {
  if (typeof fn === 'function') {
    return this._infoTransformers.push(fn);
  }

  // private implementation that traverses the chain of transformers,
  // attempting to transform auth info
  var info = fn;

  // For backwards compatibility
  if (typeof req === 'function') {
    done = req;
    req = undefined;
  }

  var stack = this._infoTransformers;
  (function pass(i, err, tinfo) {
    // transformers use 'pass' as an error to skip processing
    if ('pass' === err) {
      err = undefined;
    }
    // an error or transformed info was obtained, done
    if (err || tinfo) { return done(err, tinfo); }

    var layer = stack[i];
    if (!layer) {
      // if no transformers are registered (or they all pass), the default
      // behavior is to use the un-transformed info as-is
      return done(null, info);
    }


    function transformed(e, t) {
      pass(i + 1, e, t);
    }

    try {
      var arity = layer.length;
      if (arity == 1) {
        // sync
        var t = layer(info);
        transformed(null, t);
      } else if (arity == 3) {
        layer(req, info, transformed);
      } else {
        layer(info, transformed);
      }
    } catch(e) {
      return done(e);
    }
  })(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.unuse"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>unuse (name)](#apidoc.element.passport.Authenticator.prototype.unuse)
- description and source-code
```javascript
unuse = function (name) {
  delete this._strategies[name];
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.Authenticator.prototype.use"></a>[function <span class="apidocSignatureSpan">passport.Authenticator.prototype.</span>use (name, strategy)](#apidoc.element.passport.Authenticator.prototype.use)
- description and source-code
```javascript
use = function (name, strategy) {
  if (!strategy) {
    strategy = name;
    name = strategy.name;
  }
  if (!name) { throw new Error('Authentication strategies must have a name'); }

  this._strategies[name] = strategy;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport.Strategy"></a>[module passport.Strategy](#apidoc.module.passport.Strategy)

#### <a name="apidoc.element.passport.Strategy.Strategy"></a>[function <span class="apidocSignatureSpan">passport.</span>Strategy ()](#apidoc.element.passport.Strategy.Strategy)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport.Strategy.prototype"></a>[module passport.Strategy.prototype](#apidoc.module.passport.Strategy.prototype)

#### <a name="apidoc.element.passport.Strategy.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport.Strategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport.Strategy.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  throw new Error('Strategy#authenticate must be overridden by subclass');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport._framework"></a>[module passport._framework](#apidoc.module.passport._framework)

#### <a name="apidoc.element.passport._framework.authenticate"></a>[function <span class="apidocSignatureSpan">passport._framework.</span>authenticate (passport, name, options, callback)](#apidoc.element.passport._framework.authenticate)
- description and source-code
```javascript
function authenticate(passport, name, options, callback) {
  if (typeof options == 'function') {
    callback = options;
    options = {};
  }
  options = options || {};

  var multi = true;

  // Cast 'name' to an array, allowing authentication to pass through a chain of
  // strategies.  The first strategy to succeed, redirect, or error will halt
  // the chain.  Authentication failures will proceed through each strategy in
  // series, ultimately failing if all strategies fail.
  //
  // This is typically used on API endpoints to allow clients to authenticate
  // using their preferred choice of Basic, Digest, token-based schemes, etc.
  // It is not feasible to construct a chain of multiple strategies that involve
  // redirection (for example both Facebook and Twitter), since the first one to
  // redirect will halt the chain.
  if (!Array.isArray(name)) {
    name = [ name ];
    multi = false;
  }

  return function authenticate(req, res, next) {
    if (http.IncomingMessage.prototype.logIn
        && http.IncomingMessage.prototype.logIn !== IncomingMessageExt.logIn) {
      require('../framework/connect').__monkeypatchNode();
    }


    // accumulator for failures from each strategy in the chain
    var failures = [];

    function allFailed() {
      if (callback) {
        if (!multi) {
          return callback(null, false, failures[0].challenge, failures[0].status);
        } else {
          var challenges = failures.map(function(f) { return f.challenge; });
          var statuses = failures.map(function(f) { return f.status; });
          return callback(null, false, challenges, statuses);
        }
      }

      // Strategies are ordered by priority.  For the purpose of flashing a
      // message, the first failure will be displayed.
      var failure = failures[0] || {}
        , challenge = failure.challenge || {}
        , msg;

      if (options.failureFlash) {
        var flash = options.failureFlash;
        if (typeof flash == 'string') {
          flash = { type: 'error', message: flash };
        }
        flash.type = flash.type || 'error';

        var type = flash.type || challenge.type || 'error';
        msg = flash.message || challenge.message || challenge;
        if (typeof msg == 'string') {
          req.flash(type, msg);
        }
      }
      if (options.failureMessage) {
        msg = options.failureMessage;
        if (typeof msg == 'boolean') {
          msg = challenge.message || challenge;
        }
        if (typeof msg == 'string') {
          req.session.messages = req.session.messages || [];
          req.session.messages.push(msg);
        }
      }
      if (options.failureRedirect) {
        return res.redirect(options.failureRedirect);
      }

      // When failure handling is not delegated to the application, the default
      // is to respond with 401 Unauthorized.  Note that the WWW-Authenticate
      // header will be set according to the strategies in use (see
      // actions#fail).  If multiple strategies failed, each of their challenges
      // will be included in the response.
      var rchallenge = []
        , rstatus, status;

      for (var j = 0, len = failures.length; j < len; j++) {
        failure = failures[j];
        challenge = failure.challenge;
        status = failure.status;

        rstatus = rstatus || status;
        if (typeof challenge == 'string') {
          rchallenge.push(challenge);
        }
      }

      res.statusCode = rstatus || 401;
      if (res.statusCode == 401 && rchallenge.length) {
        res.setHeader('WWW-Authenticate', rchallenge);
      }
      if (options.failWithError) {
        return next(new AuthenticationError(http.STATUS_CODES[res.statusCode], rstatus));
      }
      res.end(http.STATUS_CODES[res.statusCode]);
    }

    (function attempt(i) {
      var layer = name[i];
      // If no more strategies exist in the chain, authentication has failed.
      if (!layer) { return allFailed(); }

      // Get the strategy, which will be used as prot ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport._framework.initialize"></a>[function <span class="apidocSignatureSpan">passport._framework.</span>initialize (passport)](#apidoc.element.passport._framework.initialize)
- description and source-code
```javascript
function initialize(passport) {

  return function initialize(req, res, next) {
    req._passport = {};
    req._passport.instance = passport;

    if (req.session && req.session[passport._key]) {
      // load data from existing session
      req._passport.session = req.session[passport._key];
    }

    next();
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport.strategies"></a>[module passport.strategies](#apidoc.module.passport.strategies)

#### <a name="apidoc.element.passport.strategies.SessionStrategy"></a>[function <span class="apidocSignatureSpan">passport.strategies.</span>SessionStrategy ()](#apidoc.element.passport.strategies.SessionStrategy)
- description and source-code
```javascript
function SessionStrategy() {
  Strategy.call(this);
  this.name = 'session';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport.strategies.SessionStrategy"></a>[module passport.strategies.SessionStrategy](#apidoc.module.passport.strategies.SessionStrategy)

#### <a name="apidoc.element.passport.strategies.SessionStrategy.SessionStrategy"></a>[function <span class="apidocSignatureSpan">passport.strategies.</span>SessionStrategy ()](#apidoc.element.passport.strategies.SessionStrategy.SessionStrategy)
- description and source-code
```javascript
function SessionStrategy() {
  Strategy.call(this);
  this.name = 'session';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport.strategies.SessionStrategy.super_"></a>[function <span class="apidocSignatureSpan">passport.strategies.SessionStrategy.</span>super_ ()](#apidoc.element.passport.strategies.SessionStrategy.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport.strategies.SessionStrategy.prototype"></a>[module passport.strategies.SessionStrategy.prototype](#apidoc.module.passport.strategies.SessionStrategy.prototype)

#### <a name="apidoc.element.passport.strategies.SessionStrategy.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport.strategies.SessionStrategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport.strategies.SessionStrategy.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  if (!req._passport) { return this.error(new Error('passport.initialize() middleware not in use')); }
  options = options || {};

  var self = this,
      su;
  if (req._passport.session) {
    su = req._passport.session.user;
  }

  if (su || su === 0) {
    // NOTE: Stream pausing is desirable in the case where later middleware is
    //       listening for events emitted from request.  For discussion on the
    //       matter, refer to: https://github.com/jaredhanson/passport/pull/106

    var paused = options.pauseStream ? pause(req) : null;
    req._passport.instance.deserializeUser(su, req, function(err, user) {
      if (err) { return self.error(err); }
      if (!user) {
        delete req._passport.session.user;
        self.pass();
        if (paused) {
          paused.resume();
        }
        return;
      }
      var property = req._passport.instance._userProperty || 'user';
      req[property] = user;
      self.pass();
      if (paused) {
        paused.resume();
      }
    });
  } else {
    self.pass();
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
