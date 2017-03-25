# api documentation for  [winston (v2.3.1)](https://github.com/winstonjs/winston#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-winston.svg)](https://travis-ci.org/npmdoc/node-npmdoc-winston)
#### A multi-transport async logging library for Node.js

[![NPM](https://nodei.co/npm/winston.png?downloads=true)](https://www.npmjs.com/package/winston)

[![apidoc](https://npmdoc.github.io/node-npmdoc-winston/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-winston_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-winston/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-winston/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins",
        "email": "charlie.robbins@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/winstonjs/winston/issues"
    },
    "dependencies": {
        "async": "~1.0.0",
        "colors": "1.0.x",
        "cycle": "1.0.x",
        "eyes": "0.1.x",
        "isstream": "0.1.x",
        "stack-trace": "0.0.x"
    },
    "description": "A multi-transport async logging library for Node.js",
    "devDependencies": {
        "cross-spawn-async": "^2.0.0",
        "hock": "1.x.x",
        "std-mocks": "~1.0.0",
        "vows": "0.7.x"
    },
    "directories": {},
    "dist": {
        "shasum": "0b48420d978c01804cf0230b648861598225a119",
        "tarball": "https://registry.npmjs.org/winston/-/winston-2.3.1.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "fba37b44f7875ba7c460df81fad27d6a941ed213",
    "homepage": "https://github.com/winstonjs/winston#readme",
    "keywords": [
        "winston",
        "logging",
        "sysadmin",
        "tools"
    ],
    "license": "MIT",
    "main": "./lib/winston",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "chjj",
            "email": "chjjeffrey@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        },
        {
            "name": "pose",
            "email": "albertopose@gmail.com"
        },
        {
            "name": "v1",
            "email": "info@3rd-Eden.com"
        },
        {
            "name": "3rdeden",
            "email": "npm@3rd-Eden.com"
        }
    ],
    "name": "winston",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/winstonjs/winston.git"
    },
    "scripts": {
        "test": "vows --spec --isolate"
    },
    "version": "2.3.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module winston](#apidoc.module.winston)
1.  [function <span class="apidocSignatureSpan">winston.</span>Container (options)](#apidoc.element.winston.Container)
1.  [function <span class="apidocSignatureSpan">winston.</span>Logger (options)](#apidoc.element.winston.Logger)
1.  [function <span class="apidocSignatureSpan">winston.</span>Transport (options)](#apidoc.element.winston.Transport)
1.  [function <span class="apidocSignatureSpan">winston.</span>add ()](#apidoc.element.winston.add)
1.  [function <span class="apidocSignatureSpan">winston.</span>addColors (colors)](#apidoc.element.winston.addColors)
1.  [function <span class="apidocSignatureSpan">winston.</span>clear ()](#apidoc.element.winston.clear)
1.  [function <span class="apidocSignatureSpan">winston.</span>cli ()](#apidoc.element.winston.cli)
1.  [function <span class="apidocSignatureSpan">winston.</span>clone (obj)](#apidoc.element.winston.clone)
1.  [function <span class="apidocSignatureSpan">winston.</span>configure ()](#apidoc.element.winston.configure)
1.  [function <span class="apidocSignatureSpan">winston.</span>debug (msg)](#apidoc.element.winston.debug)
1.  [function <span class="apidocSignatureSpan">winston.</span>error (msg)](#apidoc.element.winston.error)
1.  [function <span class="apidocSignatureSpan">winston.</span>extend ()](#apidoc.element.winston.extend)
1.  [function <span class="apidocSignatureSpan">winston.</span>handleExceptions ()](#apidoc.element.winston.handleExceptions)
1.  [function <span class="apidocSignatureSpan">winston.</span>hash (str)](#apidoc.element.winston.hash)
1.  [function <span class="apidocSignatureSpan">winston.</span>info (msg)](#apidoc.element.winston.info)
1.  [function <span class="apidocSignatureSpan">winston.</span>log ()](#apidoc.element.winston.log)
1.  [function <span class="apidocSignatureSpan">winston.</span>longestElement (xs)](#apidoc.element.winston.longestElement)
1.  [function <span class="apidocSignatureSpan">winston.</span>profile ()](#apidoc.element.winston.profile)
1.  [function <span class="apidocSignatureSpan">winston.</span>query ()](#apidoc.element.winston.query)
1.  [function <span class="apidocSignatureSpan">winston.</span>remove ()](#apidoc.element.winston.remove)
1.  [function <span class="apidocSignatureSpan">winston.</span>setLevels (target)](#apidoc.element.winston.setLevels)
1.  [function <span class="apidocSignatureSpan">winston.</span>silly (msg)](#apidoc.element.winston.silly)
1.  [function <span class="apidocSignatureSpan">winston.</span>startTimer ()](#apidoc.element.winston.startTimer)
1.  [function <span class="apidocSignatureSpan">winston.</span>stream ()](#apidoc.element.winston.stream)
1.  [function <span class="apidocSignatureSpan">winston.</span>transports.Console (options)](#apidoc.element.winston.transports.Console)
1.  [function <span class="apidocSignatureSpan">winston.</span>transports.File (options)](#apidoc.element.winston.transports.File)
1.  [function <span class="apidocSignatureSpan">winston.</span>transports.Http (options)](#apidoc.element.winston.transports.Http)
1.  [function <span class="apidocSignatureSpan">winston.</span>transports.Memory (options)](#apidoc.element.winston.transports.Memory)
1.  [function <span class="apidocSignatureSpan">winston.</span>unhandleExceptions ()](#apidoc.element.winston.unhandleExceptions)
1.  [function <span class="apidocSignatureSpan">winston.</span>verbose (msg)](#apidoc.element.winston.verbose)
1.  [function <span class="apidocSignatureSpan">winston.</span>warn (msg)](#apidoc.element.winston.warn)
1.  object <span class="apidocSignatureSpan">winston.</span>Container.prototype
1.  object <span class="apidocSignatureSpan">winston.</span>Logger.prototype
1.  object <span class="apidocSignatureSpan">winston.</span>Transport.prototype
1.  object <span class="apidocSignatureSpan">winston.</span>config
1.  object <span class="apidocSignatureSpan">winston.</span>exception
1.  object <span class="apidocSignatureSpan">winston.</span>levels
1.  object <span class="apidocSignatureSpan">winston.</span>loggers
1.  object <span class="apidocSignatureSpan">winston.</span>transports
1.  object <span class="apidocSignatureSpan">winston.</span>transports.Console.prototype
1.  object <span class="apidocSignatureSpan">winston.</span>transports.File.prototype
1.  object <span class="apidocSignatureSpan">winston.</span>transports.Http.prototype
1.  object <span class="apidocSignatureSpan">winston.</span>transports.Memory.prototype
1.  string <span class="apidocSignatureSpan">winston.</span>version

#### [module winston.Container](#apidoc.module.winston.Container)
1.  [function <span class="apidocSignatureSpan">winston.</span>Container (options)](#apidoc.element.winston.Container.Container)

#### [module winston.Container.prototype](#apidoc.module.winston.Container.prototype)
1.  [function <span class="apidocSignatureSpan">winston.Container.prototype.</span>_delete (id)](#apidoc.element.winston.Container.prototype._delete)
1.  [function <span class="apidocSignatureSpan">winston.Container.prototype.</span>add (id, options)](#apidoc.element.winston.Container.prototype.add)
1.  [function <span class="apidocSignatureSpan">winston.Container.prototype.</span>close (id)](#apidoc.element.winston.Container.prototype.close)
1.  [function <span class="apidocSignatureSpan">winston.Container.prototype.</span>get (id, options)](#apidoc.element.winston.Container.prototype.get)
1.  [function <span class="apidocSignatureSpan">winston.Container.prototype.</span>has (id)](#apidoc.element.winston.Container.prototype.has)

#### [module winston.Logger](#apidoc.module.winston.Logger)
1.  [function <span class="apidocSignatureSpan">winston.</span>Logger (options)](#apidoc.element.winston.Logger.Logger)
1.  [function <span class="apidocSignatureSpan">winston.Logger.</span>super_ ()](#apidoc.element.winston.Logger.super_)

#### [module winston.Logger.prototype](#apidoc.module.winston.Logger.prototype)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>_getExceptionHandlers ()](#apidoc.element.winston.Logger.prototype._getExceptionHandlers)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>_onError (transport, err)](#apidoc.element.winston.Logger.prototype._onError)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>_uncaughtException (err)](#apidoc.element.winston.Logger.prototype._uncaughtException)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>add (transport, options, created)](#apidoc.element.winston.Logger.prototype.add)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>clear ()](#apidoc.element.winston.Logger.prototype.clear)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>cli ()](#apidoc.element.winston.Logger.prototype.cli)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>close ()](#apidoc.element.winston.Logger.prototype.close)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>configure (options)](#apidoc.element.winston.Logger.prototype.configure)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>handleExceptions ()](#apidoc.element.winston.Logger.prototype.handleExceptions)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>log (level)](#apidoc.element.winston.Logger.prototype.log)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>profile (id)](#apidoc.element.winston.Logger.prototype.profile)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>query (options, callback)](#apidoc.element.winston.Logger.prototype.query)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>remove (transport)](#apidoc.element.winston.Logger.prototype.remove)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>setLevels (target)](#apidoc.element.winston.Logger.prototype.setLevels)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>startTimer ()](#apidoc.element.winston.Logger.prototype.startTimer)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>stream (options)](#apidoc.element.winston.Logger.prototype.stream)
1.  [function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>unhandleExceptions ()](#apidoc.element.winston.Logger.prototype.unhandleExceptions)

#### [module winston.Transport](#apidoc.module.winston.Transport)
1.  [function <span class="apidocSignatureSpan">winston.</span>Transport (options)](#apidoc.element.winston.Transport.Transport)
1.  [function <span class="apidocSignatureSpan">winston.Transport.</span>super_ ()](#apidoc.element.winston.Transport.super_)

#### [module winston.Transport.prototype](#apidoc.module.winston.Transport.prototype)
1.  [function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>formatQuery (query)](#apidoc.element.winston.Transport.prototype.formatQuery)
1.  [function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>formatResults (results, options)](#apidoc.element.winston.Transport.prototype.formatResults)
1.  [function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>logException (msg, meta, callback)](#apidoc.element.winston.Transport.prototype.logException)
1.  [function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>normalizeQuery (options)](#apidoc.element.winston.Transport.prototype.normalizeQuery)

#### [module winston.config](#apidoc.module.winston.config)
1.  [function <span class="apidocSignatureSpan">winston.config.</span>addColors (colors)](#apidoc.element.winston.config.addColors)
1.  [function <span class="apidocSignatureSpan">winston.config.</span>colorize (level, message)](#apidoc.element.winston.config.colorize)
1.  object <span class="apidocSignatureSpan">winston.config.</span>allColors
1.  object <span class="apidocSignatureSpan">winston.config.</span>cli
1.  object <span class="apidocSignatureSpan">winston.config.</span>npm
1.  object <span class="apidocSignatureSpan">winston.config.</span>syslog

#### [module winston.exception](#apidoc.module.winston.exception)
1.  [function <span class="apidocSignatureSpan">winston.exception.</span>getAllInfo (err)](#apidoc.element.winston.exception.getAllInfo)
1.  [function <span class="apidocSignatureSpan">winston.exception.</span>getOsInfo ()](#apidoc.element.winston.exception.getOsInfo)
1.  [function <span class="apidocSignatureSpan">winston.exception.</span>getProcessInfo ()](#apidoc.element.winston.exception.getProcessInfo)
1.  [function <span class="apidocSignatureSpan">winston.exception.</span>getTrace (err)](#apidoc.element.winston.exception.getTrace)

#### [module winston.transports](#apidoc.module.winston.transports)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>Console (options)](#apidoc.element.winston.transports.Console)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>File (options)](#apidoc.element.winston.transports.File)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>Http (options)](#apidoc.element.winston.transports.Http)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>Memory (options)](#apidoc.element.winston.transports.Memory)

#### [module winston.transports.Console](#apidoc.module.winston.transports.Console)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>Console (options)](#apidoc.element.winston.transports.Console.Console)
1.  [function <span class="apidocSignatureSpan">winston.transports.Console.</span>super_ (options)](#apidoc.element.winston.transports.Console.super_)

#### [module winston.transports.Console.prototype](#apidoc.module.winston.transports.Console.prototype)
1.  [function <span class="apidocSignatureSpan">winston.transports.Console.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.Console.prototype.log)
1.  string <span class="apidocSignatureSpan">winston.transports.Console.prototype.</span>name

#### [module winston.transports.File](#apidoc.module.winston.transports.File)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>File (options)](#apidoc.element.winston.transports.File.File)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.</span>super_ (options)](#apidoc.element.winston.transports.File.super_)

#### [module winston.transports.File.prototype](#apidoc.module.winston.transports.File.prototype)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_checkMaxFilesIncrementing (ext, basename, callback)](#apidoc.element.winston.transports.File.prototype._checkMaxFilesIncrementing)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_checkMaxFilesTailable (ext, basename, callback)](#apidoc.element.winston.transports.File.prototype._checkMaxFilesTailable)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_createStream ()](#apidoc.element.winston.transports.File.prototype._createStream)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_getFile ()](#apidoc.element.winston.transports.File.prototype._getFile)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_incFile (callback)](#apidoc.element.winston.transports.File.prototype._incFile)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_lazyDrain ()](#apidoc.element.winston.transports.File.prototype._lazyDrain)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_write (data, callback)](#apidoc.element.winston.transports.File.prototype._write)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>close ()](#apidoc.element.winston.transports.File.prototype.close)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>flush ()](#apidoc.element.winston.transports.File.prototype.flush)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.File.prototype.log)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>open (callback)](#apidoc.element.winston.transports.File.prototype.open)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>query (options, callback)](#apidoc.element.winston.transports.File.prototype.query)
1.  [function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>stream (options)](#apidoc.element.winston.transports.File.prototype.stream)
1.  string <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>name

#### [module winston.transports.Http](#apidoc.module.winston.transports.Http)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>Http (options)](#apidoc.element.winston.transports.Http.Http)
1.  [function <span class="apidocSignatureSpan">winston.transports.Http.</span>super_ (options)](#apidoc.element.winston.transports.Http.super_)

#### [module winston.transports.Http.prototype](#apidoc.module.winston.transports.Http.prototype)
1.  [function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>_request (options, callback)](#apidoc.element.winston.transports.Http.prototype._request)
1.  [function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.Http.prototype.log)
1.  [function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>query (options, callback)](#apidoc.element.winston.transports.Http.prototype.query)
1.  [function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>stream (options)](#apidoc.element.winston.transports.Http.prototype.stream)
1.  string <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>name

#### [module winston.transports.Memory](#apidoc.module.winston.transports.Memory)
1.  [function <span class="apidocSignatureSpan">winston.transports.</span>Memory (options)](#apidoc.element.winston.transports.Memory.Memory)
1.  [function <span class="apidocSignatureSpan">winston.transports.Memory.</span>super_ (options)](#apidoc.element.winston.transports.Memory.super_)

#### [module winston.transports.Memory.prototype](#apidoc.module.winston.transports.Memory.prototype)
1.  [function <span class="apidocSignatureSpan">winston.transports.Memory.prototype.</span>clearLogs ()](#apidoc.element.winston.transports.Memory.prototype.clearLogs)
1.  [function <span class="apidocSignatureSpan">winston.transports.Memory.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.Memory.prototype.log)
1.  string <span class="apidocSignatureSpan">winston.transports.Memory.prototype.</span>name



# <a name="apidoc.module.winston"></a>[module winston](#apidoc.module.winston)

#### <a name="apidoc.element.winston.Container"></a>[function <span class="apidocSignatureSpan">winston.</span>Container (options)](#apidoc.element.winston.Container)
- description and source-code
```javascript
Container = function (options) {
  this.loggers = {};
  this.options = options || {};
  this.default = {
    transports: [
      new winston.transports.Console({
        level: 'silly',
        colorize: false
      })
    ]
  }
}
```
- example usage
```shell
...
category1.info('logging from your IoC container-based logger');
'''

If you prefer to manage the 'Container' yourself you can simply instantiate one:

''' js
var winston = require('winston'),
    container = new winston.Container();

container.add('category1', {
  console: {
    level: 'silly',
    colorize: true
  },
  file: {
...
```

#### <a name="apidoc.element.winston.Logger"></a>[function <span class="apidocSignatureSpan">winston.</span>Logger (options)](#apidoc.element.winston.Logger)
- description and source-code
```javascript
Logger = function (options) {
  events.EventEmitter.call(this);
  this.configure(options);
}
```
- example usage
```shell
...
  .add(winston.transports.File)
  .remove(winston.transports.Console);
'''

You can also wholesale reconfigure a 'winston.Logger' instance using the 'configure' method:

''' js
var logger = new winston.Logger({
  level: 'info',
  transports: [
    new (winston.transports.Console)(),
    new (winston.transports.File)({ filename: 'somefile.log' })
  ]
});
...
```

#### <a name="apidoc.element.winston.Transport"></a>[function <span class="apidocSignatureSpan">winston.</span>Transport (options)](#apidoc.element.winston.Transport)
- description and source-code
```javascript
Transport = function (options) {
  events.EventEmitter.call(this);

  options        = options        || {};
  this.silent    = options.silent || false;
  this.raw       = options.raw    || false;
  this.name      = options.name   || this.name;
  this.formatter = options.formatter;

  //
  // Do not set a default level. When 'level' is falsey on any
  // 'Transport' instance, any 'Logger' instance uses the
  // configured level (instead of the Transport level)
  //
  this.level = options.level;

  this.handleExceptions = options.handleExceptions || false;
  this.exceptionsLevel  = options.exceptionsLevel || 'error';
  this.humanReadableUnhandledException = options.humanReadableUnhandledException || false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.add"></a>[function <span class="apidocSignatureSpan">winston.</span>add ()](#apidoc.element.winston.add)
- description and source-code
```javascript
add = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...
winston.level = 'debug';
winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:

''' js
winston.add(winston.transports.File, { filename: 'somefile.log' });
winston.remove(winston.transports.Console);
'''

Or do it with one call to configure():

''' js
winston.configure({
...
```

#### <a name="apidoc.element.winston.addColors"></a>[function <span class="apidocSignatureSpan">winston.</span>addColors (colors)](#apidoc.element.winston.addColors)
- description and source-code
```javascript
addColors = function (colors) {
  mixin(allColors, colors);
}
```
- example usage
```shell
...

Although there is slight repetition in this data structure, it enables simple encapsulation if you do not want to have colors. If
 you do wish to have colors, in addition to passing the levels to the Logger itself, you must make winston aware of them:

''' js
  //
  // Make winston aware of these colors
  //
  winston.addColors(myCustomLevels.colors);
'''

This enables transports with the 'colorize' option set to appropriately color the output of custom levels.

## Further Reading

### Events and Callbacks in Winston
...
```

#### <a name="apidoc.element.winston.clear"></a>[function <span class="apidocSignatureSpan">winston.</span>clear ()](#apidoc.element.winston.clear)
- description and source-code
```javascript
clear = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.cli"></a>[function <span class="apidocSignatureSpan">winston.</span>cli ()](#apidoc.element.winston.cli)
- description and source-code
```javascript
cli = function () {
  winston.padLevels = true;
  common.setLevels(winston, defaultLogger.levels, winston.config.cli.levels);
  defaultLogger.setLevels(winston.config.cli.levels);
  winston.config.addColors(winston.config.cli.colors);

  if (defaultLogger.transports.console) {
    defaultLogger.transports.console.colorize = true;
    defaultLogger.transports.console.timestamp = false;
  }

  return winston;
}
```
- example usage
```shell
...
data:   }
info:   Analyzing dependencies...
info:   Done analyzing raw dependencies
info:   Retrieved packages from npm
warn:   No additional dependencies found
'''

Configuring output for this style is easy, just use the '.cli()' method on 'winston' or an instance of 'winston.Logger':

''' js
var winston = require('winston');

//
// Configure CLI output on the default logger
//
...
```

#### <a name="apidoc.element.winston.clone"></a>[function <span class="apidocSignatureSpan">winston.</span>clone (obj)](#apidoc.element.winston.clone)
- description and source-code
```javascript
clone = function (obj) {
  //
  // We only need to clone reference types (Object)
  //
  var copy = {};

  if (obj instanceof Error) {
    // With potential custom Error objects, this might not be exactly correct,
    // but probably close-enough for purposes of this lib.
    copy = { message: obj.message };
    Object.getOwnPropertyNames(obj).forEach(function (key) {
      copy[key] = obj[key];
    });

    return copy;
  }
  else if (!(obj instanceof Object)) {
    return obj;
  }
  else if (obj instanceof Date) {
    return new Date(obj.getTime());
  }

  for (var i in obj) {
    if (Array.isArray(obj[i])) {
      copy[i] = obj[i].slice(0);
    }
    else if (obj[i] instanceof Buffer) {
        copy[i] = obj[i].slice(0);
    }
    else if (typeof obj[i] != 'function') {
      copy[i] = obj[i] instanceof Object ? exports.clone(obj[i]) : obj[i];
    }
    else if (typeof obj[i] === 'function') {
      copy[i] = obj[i];
    }
  }

  return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.configure"></a>[function <span class="apidocSignatureSpan">winston.</span>configure ()](#apidoc.element.winston.configure)
- description and source-code
```javascript
configure = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...
  winston.add(winston.transports.File, { filename: 'somefile.log' });
  winston.remove(winston.transports.Console);
'''

Or do it with one call to configure():

''' js
  winston.configure({
    transports: [
      new (winston.transports.File)({ filename: 'somefile.log' })
    ]
  });
'''

For more documentation about working with each individual transport supported by Winston see the [Winston Transports](docs/transports
.md) document.
...
```

#### <a name="apidoc.element.winston.debug"></a>[function <span class="apidocSignatureSpan">winston.</span>debug (msg)](#apidoc.element.winston.debug)
- description and source-code
```javascript
debug = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
''' js
  var logger = new (winston.Logger)({
    transports: [
      new (winston.transports.Console)({ level: 'warn' }),
      new (winston.transports.File)({ filename: 'somefile.log', level: 'error' })
    ]
  });
  logger.debug("Will not be logged in either transport!");
  logger.transports.console.level = 'debug';
  logger.transports.file.level = 'verbose';
  logger.verbose("Will be logged in both transports!");
'''

As of 0.2.0, winston supports customizable logging levels, defaulting to [npm][0] style logging levels. Changing logging levels
is easy:
...
```

#### <a name="apidoc.element.winston.error"></a>[function <span class="apidocSignatureSpan">winston.</span>error (msg)](#apidoc.element.winston.error)
- description and source-code
```javascript
error = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
  logger.log('debug', "127.0.0.1 - there's no place like home");
  logger.log('verbose', "127.0.0.1 - there's no place like home");
  logger.log('info', "127.0.0.1 - there's no place like home");
  logger.log('warn', "127.0.0.1 - there's no place like home");
  logger.log('error', "127.0.0.1 - there's no place like home");
  logger.info("127.0.0.1 - there's no place like home");
  logger.warn("127.0.0.1 - there's no place like home");
  logger.error("127.0.0.1 - there's no place like home");

  //
  // Default logger
  //
  winston.log('info', "127.0.0.1 - there's no place like home");
  winston.info("127.0.0.1 - there's no place like home");
'''
...
```

#### <a name="apidoc.element.winston.extend"></a>[function <span class="apidocSignatureSpan">winston.</span>extend ()](#apidoc.element.winston.extend)
- description and source-code
```javascript
extend = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.handleExceptions"></a>[function <span class="apidocSignatureSpan">winston.</span>handleExceptions ()](#apidoc.element.winston.handleExceptions)
- description and source-code
```javascript
handleExceptions = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...

## Exceptions

### Handling Uncaught Exceptions with winston

With 'winston', it is possible to catch and log 'uncaughtException' events from your process. There are two distinct ways of enabling
 this functionality either through the default winston logger or your own logger instance.

If you want to use this feature with the default logger simply call '.handleExceptions()' with a transport instance.

''' js
//
// You can add a separate exception logger by passing it to '.handleExceptions'
//
winston.handleExceptions(new winston.transports.File({ filename: 'path/to/exceptions.log' }))
...
```

#### <a name="apidoc.element.winston.hash"></a>[function <span class="apidocSignatureSpan">winston.</span>hash (str)](#apidoc.element.winston.hash)
- description and source-code
```javascript
hash = function (str) {
  return crypto.createHash('sha1').update(str).digest('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.info"></a>[function <span class="apidocSignatureSpan">winston.</span>info (msg)](#apidoc.element.winston.info)
- description and source-code
```javascript
info = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
### Using the Default Logger
The default logger is accessible through the winston module directly. Any method that you could call on an instance of a logger
is available on the default logger:

''' js
  var winston = require('winston');

  winston.log('info', 'Hello distributed log files!');
  winston.info('Hello again distributed logs');

  winston.level = 'debug';
  winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:
...
```

#### <a name="apidoc.element.winston.log"></a>[function <span class="apidocSignatureSpan">winston.</span>log ()](#apidoc.element.winston.log)
- description and source-code
```javascript
log = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...

### Using the Default Logger
The default logger is accessible through the winston module directly. Any method that you could call on an instance of a logger
is available on the default logger:

''' js
  var winston = require('winston');

  winston.log('info', 'Hello distributed log files!');
  winston.info('Hello again distributed logs');

  winston.level = 'debug';
  winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:
...
```

#### <a name="apidoc.element.winston.longestElement"></a>[function <span class="apidocSignatureSpan">winston.</span>longestElement (xs)](#apidoc.element.winston.longestElement)
- description and source-code
```javascript
longestElement = function (xs) {
  return Math.max.apply(
    null,
    xs.map(function (x) { return x.length; })
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.profile"></a>[function <span class="apidocSignatureSpan">winston.</span>profile ()](#apidoc.element.winston.profile)
- description and source-code
```javascript
profile = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...
In addition to logging messages and metadata, winston also has a simple profiling mechanism implemented for any logger:

''' js
//
// Start profile of 'test'
// Remark: Consider using Date.now() with async operations
//
winston.profile('test');

setTimeout(function () {
  //
  // Stop profile of 'test'. Logging will now take place:
  //   "17 Jan 21:00:00 - info: test duration=1000ms"
  //
  winston.profile('test');
...
```

#### <a name="apidoc.element.winston.query"></a>[function <span class="apidocSignatureSpan">winston.</span>query ()](#apidoc.element.winston.query)
- description and source-code
```javascript
query = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...
    order: 'desc',
    fields: ['message']
  };

  //
  // Find items logged between today and yesterday.
  //
  winston.query(options, function (err, results) {
    if (err) {
      throw err;
    }

    console.log(results);
  });
'''
...
```

#### <a name="apidoc.element.winston.remove"></a>[function <span class="apidocSignatureSpan">winston.</span>remove ()](#apidoc.element.winston.remove)
- description and source-code
```javascript
remove = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...
winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:

''' js
winston.add(winston.transports.File, { filename: 'somefile.log' });
winston.remove(winston.transports.Console);
'''

Or do it with one call to configure():

''' js
winston.configure({
  transports: [
...
```

#### <a name="apidoc.element.winston.setLevels"></a>[function <span class="apidocSignatureSpan">winston.</span>setLevels (target)](#apidoc.element.winston.setLevels)
- description and source-code
```javascript
setLevels = function (target) {
  common.setLevels(winston, defaultLogger.levels, target);
  defaultLogger.setLevels(target);
}
```
- example usage
```shell
...

As of 0.2.0, winston supports customizable logging levels, defaulting to [npm][0] style logging levels. Changing logging levels
is easy:

''' js
  //
  // Change levels on the default winston logger
  //
  winston.setLevels(winston.config.syslog.levels);

  //
  // Change levels on an instance of a logger
  //
  logger.setLevels(winston.config.syslog.levels);
'''
...
```

#### <a name="apidoc.element.winston.silly"></a>[function <span class="apidocSignatureSpan">winston.</span>silly (msg)](#apidoc.element.winston.silly)
- description and source-code
```javascript
silly = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...

Calling '.setLevels' on a logger will remove all of the previous helper methods for the old levels and define helper methods for
 the new levels. Thus, you should be careful about the logging statements you use when changing levels. For example, if you ran
this code after changing to the syslog levels:

''' js
//
// Logger does not have 'silly' defined since that level is not in the syslog levels
//
logger.silly('some silly message');
'''

### Using Custom Logging Levels
In addition to the predefined 'npm' and 'syslog' levels available in Winston, you can also choose to define your own:

''' js
var myCustomLevels = {
...
```

#### <a name="apidoc.element.winston.startTimer"></a>[function <span class="apidocSignatureSpan">winston.</span>startTimer ()](#apidoc.element.winston.startTimer)
- description and source-code
```javascript
startTimer = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.stream"></a>[function <span class="apidocSignatureSpan">winston.</span>stream ()](#apidoc.element.winston.stream)
- description and source-code
```javascript
stream = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
...
## Streaming Logs
Streaming allows you to stream your logs back from your chosen transport.

''' js
  //
  // Start at the end.
  //
  winston.stream({ start: -1 }).on('log', function(log) {
    console.log(log);
  });
'''

## Exceptions

### Handling Uncaught Exceptions with winston
...
```

#### <a name="apidoc.element.winston.transports.Console"></a>[function <span class="apidocSignatureSpan">winston.</span>transports.Console (options)](#apidoc.element.winston.transports.Console)
- description and source-code
```javascript
transports.Console = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.json         = options.json        || false;
  this.colorize     = options.colorize    || false;
  this.prettyPrint  = options.prettyPrint || false;
  this.timestamp    = typeof options.timestamp !== 'undefined' ? options.timestamp : false;
  this.showLevel    = options.showLevel === undefined ? true : options.showLevel;
  this.label        = options.label       || null;
  this.logstash     = options.logstash    || false;
  this.depth        = options.depth       || null;
  this.align        = options.align       || false;
  this.stderrLevels = setStderrLevels(options.stderrLevels, options.debugStdout);
  this.eol          = options.eol   || os.EOL;

  if (this.json) {
    this.stringify = options.stringify || function (obj) {
      return JSON.stringify(obj, null, 2);
    };
  }

  //
  // Convert stderrLevels into an Object for faster key-lookup times than an Array.
  //
  // For backwards compatibility, stderrLevels defaults to ['error', 'debug']
  // or ['error'] depending on whether options.debugStdout is true.
  //
  function setStderrLevels (levels, debugStdout) {
    var defaultMsg = 'Cannot have non-string elements in stderrLevels Array';
    if (debugStdout) {
      if (levels) {
        //
        // Don't allow setting both debugStdout and stderrLevels together,
        // since this could cause behaviour a programmer might not expect.
        //
        throw new Error('Cannot set debugStdout and stderrLevels together');
      }

      return common.stringArrayToSet(['error'], defaultMsg);
    }

    if (!levels) {
      return common.stringArrayToSet(['error', 'debug'], defaultMsg);
    } else if (!(Array.isArray(levels))) {
      throw new Error('Cannot set stderrLevels to type other than Array');
    }

    return common.stringArrayToSet(levels, defaultMsg);
  };
}
```
- example usage
```shell
...
'''

Example 2

''' js
var logger = new winston.Logger({
  transports: [
    new winston.transports.Console({
      handleExceptions: true,
      json: true
    })
  ],
  exitOnError: false
});
'''
...
```

#### <a name="apidoc.element.winston.transports.File"></a>[function <span class="apidocSignatureSpan">winston.</span>transports.File (options)](#apidoc.element.winston.transports.File)
- description and source-code
```javascript
transports.File = function (options) {
  var self = this;
  Transport.call(this, options);

  //
  // Helper function which throws an 'Error' in the event
  // that any of the rest of the arguments is present in 'options'.
  //
  function throwIf (target /*, illegal... */) {
    Array.prototype.slice.call(arguments, 1).forEach(function (name) {
      if (options[name]) {
        throw new Error('Cannot set ' + name + ' and ' + target + 'together');
      }
    });
  }

  if (options.filename || options.dirname) {
    throwIf('filename or dirname', 'stream');
    this._basename = this.filename = options.filename
      ? path.basename(options.filename)
      : 'winston.log';

    this.dirname = options.dirname || path.dirname(options.filename);
    this.options = options.options || { flags: 'a' };

    //
    // "24 bytes" is maybe a good value for logging lines.
    //
    this.options.highWaterMark = this.options.highWaterMark || 24;
  }
  else if (options.stream) {
    throwIf('stream', 'filename', 'maxsize');
    this._stream = options.stream;
    this._isStreams2 = isWritable(this._stream);
    this._stream.on('error', function(error){
      self.emit('error', error);
    });
    //
    // We need to listen for drain events when
    // write() returns false. This can make node
    // mad at times.
    //
    this._stream.setMaxListeners(Infinity);
  }
  else {
    throw new Error('Cannot log to file without filename or stream.');
  }

  this.json        = options.json !== false;
  this.logstash    = options.logstash    || false;
  this.colorize    = options.colorize    || false;
  this.maxsize     = options.maxsize     || null;
  this.rotationFormat = options.rotationFormat || false;
  this.zippedArchive = options.zippedArchive || false;
  this.maxFiles    = options.maxFiles    || null;
  this.prettyPrint = options.prettyPrint || false;
  this.label       = options.label       || null;
  this.timestamp   = options.timestamp != null ? options.timestamp : true;
  this.eol         = options.eol || os.EOL;
  this.tailable    = options.tailable    || false;
  this.depth       = options.depth       || null;
  this.showLevel   = options.showLevel === undefined ? true : options.showLevel;
  this.maxRetries  = options.maxRetries || 2;

  if (this.json) {
    this.stringify = options.stringify;
  }

  //
  // Internal state variables representing the number
  // of files this instance has created and the current
  // size (in bytes) of the current logfile.
  //
  this._size     = 0;
  this._created  = 0;
  this._buffer   = [];
  this._draining = false;
  this._opening  = false;
  this._failures = 0;
  this._archive = null;
}
```
- example usage
```shell
...

If you want to use this feature with the default logger simply call '.handleExceptions()' with a transport instance.

''' js
//
// You can add a separate exception logger by passing it to '.handleExceptions'
//
winston.handleExceptions(new winston.transports.File({ filename: 'path/to/exceptions.log' }))

//
// Alternatively you can set '.handleExceptions' to true when adding transports to winston.
// You can use the '.humanReadableUnhandledException' option to get more readable exceptions.
//
winston.add(winston.transports.File, {
  filename: 'path/to/all-logs.log',
...
```

#### <a name="apidoc.element.winston.transports.Http"></a>[function <span class="apidocSignatureSpan">winston.</span>transports.Http (options)](#apidoc.element.winston.transports.Http)
- description and source-code
```javascript
transports.Http = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.name = 'http';
  this.ssl = !!options.ssl;
  this.host = options.host || 'localhost';
  this.port = options.port;
  this.auth = options.auth;
  this.path = options.path || '';
  this.agent = options.agent;

  if (!this.port) {
    this.port = this.ssl ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.Memory"></a>[function <span class="apidocSignatureSpan">winston.</span>transports.Memory (options)](#apidoc.element.winston.transports.Memory)
- description and source-code
```javascript
transports.Memory = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.errorOutput = [];
  this.writeOutput = [];

  this.json        = options.json        || false;
  this.colorize    = options.colorize    || false;
  this.prettyPrint = options.prettyPrint || false;
  this.timestamp   = typeof options.timestamp !== 'undefined' ? options.timestamp : false;
  this.showLevel   = options.showLevel === undefined ? true : options.showLevel;
  this.label       = options.label       || null;
  this.depth       = options.depth       || null;

  if (this.json) {
    this.stringify = options.stringify || function (obj) {
      return JSON.stringify(obj, null, 2);
    };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.unhandleExceptions"></a>[function <span class="apidocSignatureSpan">winston.</span>unhandleExceptions ()](#apidoc.element.winston.unhandleExceptions)
- description and source-code
```javascript
unhandleExceptions = function () {
  return defaultLogger[method].apply(defaultLogger, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.verbose"></a>[function <span class="apidocSignatureSpan">winston.</span>verbose (msg)](#apidoc.element.winston.verbose)
- description and source-code
```javascript
verbose = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
    new (winston.transports.Console)({ level: 'warn' }),
    new (winston.transports.File)({ filename: 'somefile.log', level: 'error' })
  ]
});
logger.debug("Will not be logged in either transport!");
logger.transports.console.level = 'debug';
logger.transports.file.level = 'verbose';
logger.verbose("Will be logged in both transports!");
'''

As of 0.2.0, winston supports customizable logging levels, defaulting to [npm][0] style logging levels. Changing logging levels
is easy:

''' js
//
// Change levels on the default winston logger
...
```

#### <a name="apidoc.element.winston.warn"></a>[function <span class="apidocSignatureSpan">winston.</span>warn (msg)](#apidoc.element.winston.warn)
- description and source-code
```javascript
warn = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
logger.log('silly', "127.0.0.1 - there's no place like home");
logger.log('debug', "127.0.0.1 - there's no place like home");
logger.log('verbose', "127.0.0.1 - there's no place like home");
logger.log('info', "127.0.0.1 - there's no place like home");
logger.log('warn', "127.0.0.1 - there's no place like home");
logger.log('error', "127.0.0.1 - there's no place like home");
logger.info("127.0.0.1 - there's no place like home");
logger.warn("127.0.0.1 - there's no place like home");
logger.error("127.0.0.1 - there's no place like home");

//
// Default logger
//
winston.log('info', "127.0.0.1 - there's no place like home");
winston.info("127.0.0.1 - there's no place like home");
...
```



# <a name="apidoc.module.winston.Container"></a>[module winston.Container](#apidoc.module.winston.Container)

#### <a name="apidoc.element.winston.Container.Container"></a>[function <span class="apidocSignatureSpan">winston.</span>Container (options)](#apidoc.element.winston.Container.Container)
- description and source-code
```javascript
Container = function (options) {
  this.loggers = {};
  this.options = options || {};
  this.default = {
    transports: [
      new winston.transports.Console({
        level: 'silly',
        colorize: false
      })
    ]
  }
}
```
- example usage
```shell
...
category1.info('logging from your IoC container-based logger');
'''

If you prefer to manage the 'Container' yourself you can simply instantiate one:

''' js
var winston = require('winston'),
    container = new winston.Container();

container.add('category1', {
  console: {
    level: 'silly',
    colorize: true
  },
  file: {
...
```



# <a name="apidoc.module.winston.Container.prototype"></a>[module winston.Container.prototype](#apidoc.module.winston.Container.prototype)

#### <a name="apidoc.element.winston.Container.prototype._delete"></a>[function <span class="apidocSignatureSpan">winston.Container.prototype.</span>_delete (id)](#apidoc.element.winston.Container.prototype._delete)
- description and source-code
```javascript
_delete = function (id) {
    delete this.loggers[id];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Container.prototype.add"></a>[function <span class="apidocSignatureSpan">winston.Container.prototype.</span>add (id, options)](#apidoc.element.winston.Container.prototype.add)
- description and source-code
```javascript
add = function (id, options) {
  var self = this,
      existing;

  if (!this.loggers[id]) {
    //
    // Remark: Simple shallow clone for configuration options in case we pass in
    // instantiated protoypal objects
    //
    options = extend({}, options || this.options || this.default);
    existing = options.transports || this.options.transports;
    //
    // Remark: Make sure if we have an array of transports we slice it to make copies
    // of those references.
    //
    options.transports = existing ? existing.slice() : [];

    if (options.transports.length === 0 && (!options || !options['console'])) {
      options.transports.push(this.default.transports[0]);
    }

    Object.keys(options).forEach(function (key) {
      if (key === 'transports') {
        return;
      }

      var name = common.capitalize(key);

      if (!winston.transports[name]) {
        throw new Error('Cannot add unknown transport: ' + name);
      }

      var namedOptions = options[key];
      namedOptions.id = id;
      options.transports.push(new (winston.transports[name])(namedOptions));
    });

    options.id = id;
    this.loggers[id] = new winston.Logger(options);

    this.loggers[id].on('close', function () {
        self._delete(id);
    });
  }

  return this.loggers[id];
}
```
- example usage
```shell
...
winston.level = 'debug';
winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:

''' js
winston.add(winston.transports.File, { filename: 'somefile.log' });
winston.remove(winston.transports.Console);
'''

Or do it with one call to configure():

''' js
winston.configure({
...
```

#### <a name="apidoc.element.winston.Container.prototype.close"></a>[function <span class="apidocSignatureSpan">winston.Container.prototype.</span>close (id)](#apidoc.element.winston.Container.prototype.close)
- description and source-code
```javascript
close = function (id) {
  var self = this;

  function _close (id) {
    if (!self.loggers[id]) {
      return;
    }

    self.loggers[id].close();
    self._delete(id);
  }

  return id ? _close(id) : Object.keys(this.loggers).forEach(function (id) {
    _close(id);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Container.prototype.get"></a>[function <span class="apidocSignatureSpan">winston.Container.prototype.</span>get (id, options)](#apidoc.element.winston.Container.prototype.get)
- description and source-code
```javascript
get = function (id, options) {
  var self = this,
      existing;

  if (!this.loggers[id]) {
    //
    // Remark: Simple shallow clone for configuration options in case we pass in
    // instantiated protoypal objects
    //
    options = extend({}, options || this.options || this.default);
    existing = options.transports || this.options.transports;
    //
    // Remark: Make sure if we have an array of transports we slice it to make copies
    // of those references.
    //
    options.transports = existing ? existing.slice() : [];

    if (options.transports.length === 0 && (!options || !options['console'])) {
      options.transports.push(this.default.transports[0]);
    }

    Object.keys(options).forEach(function (key) {
      if (key === 'transports') {
        return;
      }

      var name = common.capitalize(key);

      if (!winston.transports[name]) {
        throw new Error('Cannot add unknown transport: ' + name);
      }

      var namedOptions = options[key];
      namedOptions.id = id;
      options.transports.push(new (winston.transports[name])(namedOptions));
    });

    options.id = id;
    this.loggers[id] = new winston.Logger(options);

    this.loggers[id].on('close', function () {
        self._delete(id);
    });
  }

  return this.loggers[id];
}
```
- example usage
```shell
...

''' js
  var winston = require('winston');

  //
  // Grab your preconfigured logger
  //
  var category1 = winston.loggers.get('category1');

  category1.info('logging from your IoC container-based logger');
'''

If you prefer to manage the 'Container' yourself you can simply instantiate one:

''' js
...
```

#### <a name="apidoc.element.winston.Container.prototype.has"></a>[function <span class="apidocSignatureSpan">winston.Container.prototype.</span>has (id)](#apidoc.element.winston.Container.prototype.has)
- description and source-code
```javascript
has = function (id) {
  return !!this.loggers[id];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.Logger"></a>[module winston.Logger](#apidoc.module.winston.Logger)

#### <a name="apidoc.element.winston.Logger.Logger"></a>[function <span class="apidocSignatureSpan">winston.</span>Logger (options)](#apidoc.element.winston.Logger.Logger)
- description and source-code
```javascript
Logger = function (options) {
  events.EventEmitter.call(this);
  this.configure(options);
}
```
- example usage
```shell
...
  .add(winston.transports.File)
  .remove(winston.transports.Console);
'''

You can also wholesale reconfigure a 'winston.Logger' instance using the 'configure' method:

''' js
var logger = new winston.Logger({
  level: 'info',
  transports: [
    new (winston.transports.Console)(),
    new (winston.transports.File)({ filename: 'somefile.log' })
  ]
});
...
```

#### <a name="apidoc.element.winston.Logger.super_"></a>[function <span class="apidocSignatureSpan">winston.Logger.</span>super_ ()](#apidoc.element.winston.Logger.super_)
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



# <a name="apidoc.module.winston.Logger.prototype"></a>[module winston.Logger.prototype](#apidoc.module.winston.Logger.prototype)

#### <a name="apidoc.element.winston.Logger.prototype._getExceptionHandlers"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>_getExceptionHandlers ()](#apidoc.element.winston.Logger.prototype._getExceptionHandlers)
- description and source-code
```javascript
_getExceptionHandlers = function () {
  var self = this;

  return this._hnames.map(function (name) {
    return self.exceptionHandlers[name];
  }).concat(this._names.map(function (name) {
    return self.transports[name].handleExceptions && self.transports[name];
  })).filter(Boolean);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Logger.prototype._onError"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>_onError (transport, err)](#apidoc.element.winston.Logger.prototype._onError)
- description and source-code
```javascript
_onError = function (transport, err) {
  if (this.emitErrs) {
    this.emit('error', err, transport);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Logger.prototype._uncaughtException"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>_uncaughtException (err)](#apidoc.element.winston.Logger.prototype._uncaughtException)
- description and source-code
```javascript
_uncaughtException = function (err) {
  var self = this,
      responded = false,
      info = exception.getAllInfo(err),
      handlers = this._getExceptionHandlers(),
      timeout,
      doExit;

  //
  // Calculate if we should exit on this error
  //
  doExit = typeof this.exitOnError === 'function'
    ? this.exitOnError(err)
    : this.exitOnError;

  function logAndWait(transport, next) {
    transport.logException('uncaughtException: ' + (err.message || err), info, next, err);
  }

  function gracefulExit() {
    if (doExit && !responded) {
      //
      // Remark: Currently ignoring any exceptions from transports
      //         when catching uncaught exceptions.
      //
      clearTimeout(timeout);
      responded = true;
      process.exit(1);
    }
  }

  if (!handlers || handlers.length === 0) {
    return gracefulExit();
  }

  //
  // Log to all transports and allow the operation to take
  // only up to '3000ms'.
  //
  async.forEach(handlers, logAndWait, gracefulExit);
  if (doExit) {
    timeout = setTimeout(gracefulExit, 3000);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Logger.prototype.add"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>add (transport, options, created)](#apidoc.element.winston.Logger.prototype.add)
- description and source-code
```javascript
add = function (transport, options, created) {
  var instance = created ? transport : (new (transport)(options));

  if (!instance.name && !instance.log) {
    throw new Error('Unknown transport with no log() method');
  }
  else if (this.transports[instance.name]) {
    throw new Error('Transport already attached: ' + instance.name + ", assign a different name");
  }

  this.transports[instance.name] = instance;
  this._names = Object.keys(this.transports);

  //
  // Listen for the 'error' event on the new Transport
  //
  instance._onError = this._onError.bind(this, instance)
  if (!created) {
    instance.on('error', instance._onError);
  }

  //
  // If this transport has 'handleExceptions' set to 'true'
  // and we are not already handling exceptions, do so.
  //
  if (instance.handleExceptions && !this.catchExceptions) {
    this.handleExceptions();
  }

  return this;
}
```
- example usage
```shell
...
winston.level = 'debug';
winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:

''' js
winston.add(winston.transports.File, { filename: 'somefile.log' });
winston.remove(winston.transports.Console);
'''

Or do it with one call to configure():

''' js
winston.configure({
...
```

#### <a name="apidoc.element.winston.Logger.prototype.clear"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>clear ()](#apidoc.element.winston.Logger.prototype.clear)
- description and source-code
```javascript
clear = function () {
  Object.keys(this.transports).forEach(function (name) {
    this.remove({ name: name });
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Logger.prototype.cli"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>cli ()](#apidoc.element.winston.Logger.prototype.cli)
- description and source-code
```javascript
cli = function () {
  this.padLevels = true;
  this.setLevels(config.cli.levels);
  config.addColors(config.cli.colors);

  if (this.transports.console) {
    this.transports.console.colorize = this.transports.console.colorize || true;
    this.transports.console.timestamp = this.transports.console.timestamp || false;
  }

  return this;
}
```
- example usage
```shell
...
data:   }
info:   Analyzing dependencies...
info:   Done analyzing raw dependencies
info:   Retrieved packages from npm
warn:   No additional dependencies found
'''

Configuring output for this style is easy, just use the '.cli()' method on 'winston' or an instance of 'winston.Logger':

''' js
var winston = require('winston');

//
// Configure CLI output on the default logger
//
...
```

#### <a name="apidoc.element.winston.Logger.prototype.close"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>close ()](#apidoc.element.winston.Logger.prototype.close)
- description and source-code
```javascript
close = function () {
  var self = this;

  this._names.forEach(function (name) {
    var transport = self.transports[name];
    if (transport && transport.close) {
      transport.close();
    }
  });

  this.emit('close');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Logger.prototype.configure"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>configure (options)](#apidoc.element.winston.Logger.prototype.configure)
- description and source-code
```javascript
configure = function (options) {
  var self = this;

  //
  // If we have already been setup with transports
  // then remove them before proceeding.
  //
  if (Array.isArray(this._names) && this._names.length) {
    this.clear();
  }

  options = options || {};
  this.transports = {};
  this._names     = [];

  if (options.transports) {
    options.transports.forEach(function (transport) {
      self.add(transport, null, true);
    });
  }

  //
  // Set Levels and default logging level
  //
  this.padLevels = options.padLevels || false;
  this.setLevels(options.levels);
  if (options.colors) {
    config.addColors(options.colors);
  }

  //
  // Hoist other options onto this instance.
  //
  this.id          = options.id || null;
  this.level       = options.level || 'info';
  this.emitErrs    = options.emitErrs || false;
  this.stripColors = options.stripColors || false;
  this.exitOnError = typeof options.exitOnError !== 'undefined'
    ? options.exitOnError
    : true;

  //
  // Setup internal state as empty Objects even though it is
  // defined lazily later to ensure a strong existential API contract.
  //
  this.exceptionHandlers = {};
  this.profilers         = {};

  ['rewriters', 'filters'].forEach(function (kind) {
    self[kind] = Array.isArray(options[kind])
      ? options[kind]
      : [];
  });

  if (options.exceptionHandlers) {
    this.handleExceptions(options.exceptionHandlers);
  }
}
```
- example usage
```shell
...
  winston.add(winston.transports.File, { filename: 'somefile.log' });
  winston.remove(winston.transports.Console);
'''

Or do it with one call to configure():

''' js
  winston.configure({
    transports: [
      new (winston.transports.File)({ filename: 'somefile.log' })
    ]
  });
'''

For more documentation about working with each individual transport supported by Winston see the [Winston Transports](docs/transports
.md) document.
...
```

#### <a name="apidoc.element.winston.Logger.prototype.handleExceptions"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>handleExceptions ()](#apidoc.element.winston.Logger.prototype.handleExceptions)
- description and source-code
```javascript
handleExceptions = function () {
  var args = Array.prototype.slice.call(arguments),
      handlers = [],
      self = this;

  args.forEach(function (a) {
    if (Array.isArray(a)) {
      handlers = handlers.concat(a);
    }
    else {
      handlers.push(a);
    }
  });

  this.exceptionHandlers = this.exceptionHandlers || {};
  handlers.forEach(function (handler) {
    self.exceptionHandlers[handler.name] = handler;
  });

  this._hnames = Object.keys(self.exceptionHandlers);

  if (!this.catchExceptions) {
    this.catchExceptions = this._uncaughtException.bind(this);
    process.on('uncaughtException', this.catchExceptions);
  }
}
```
- example usage
```shell
...

## Exceptions

### Handling Uncaught Exceptions with winston

With 'winston', it is possible to catch and log 'uncaughtException' events from your process. There are two distinct ways of enabling
 this functionality either through the default winston logger or your own logger instance.

If you want to use this feature with the default logger simply call '.handleExceptions()' with a transport instance.

''' js
//
// You can add a separate exception logger by passing it to '.handleExceptions'
//
winston.handleExceptions(new winston.transports.File({ filename: 'path/to/exceptions.log' }))
...
```

#### <a name="apidoc.element.winston.Logger.prototype.log"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>log (level)](#apidoc.element.winston.Logger.prototype.log)
- description and source-code
```javascript
log = function (level) {
  var args = Array.prototype.slice.call(arguments, 1),
      self = this,
      transports;

  while (args[args.length - 1] === null) {
    args.pop();
  }

  //
  // Determining what is 'meta' and what are arguments for string interpolation
  // turns out to be VERY tricky. e.g. in the cases like this:
  //
  //    logger.info('No interpolation symbols', 'ok', 'why', { meta: 'is-this' });
  //
  var callback  = typeof args[args.length - 1] === 'function'
    ? args.pop()
    : null;

  //
  // Handle errors appropriately.
  //
  function onError(err) {
    if (callback) {
      callback(err);
    }
    else if (self.emitErrs) {
      self.emit('error', err);
    }
  }

  if (this._names.length === 0) {
    return onError(new Error('Cannot log with no transports.'));
  }
  else if (typeof self.levels[level] === 'undefined') {
    return onError(new Error('Unknown log level: ' + level));
  }

  //
  // If there are no transports that match the level
  // then be eager and return. This could potentially be calculated
  // during 'setLevels' for more performance gains.
  //
  var targets = this._names.filter(function (name) {
    var transport = self.transports[name];
    return (transport.level && self.levels[transport.level] >= self.levels[level])
      || (!transport.level && self.levels[self.level] >= self.levels[level]);
  });

  if (!targets.length) {
    if (callback) { callback(); }
    return;
  }

  //
  // Determining what is 'meta' and what are arguments for string interpolation
  // turns out to be VERY tricky. e.g. in the cases like this:
  //
  //    logger.info('No interpolation symbols', 'ok', 'why', { meta: 'is-this' });
  //
  var msg, meta = {}, validMeta = false;
  var hasFormat = args && args[0] && args[0].match && args[0].match(formatRegExp) !== null;
  var tokens = (hasFormat) ? args[0].match(formatRegExp) : [];
  var ptokens = tokens.filter(function(t) { return t === '%%' });
  if (((args.length - 1) - (tokens.length - ptokens.length)) > 0 || args.length === 1) {
    // last arg is meta
    meta = args[args.length - 1] || args;
    var metaType = Object.prototype.toString.call(meta);
    validMeta = metaType === '[object Object]' ||
      metaType === '[object Error]' || metaType === '[object Array]';
    meta = validMeta ? args.pop() : {};
  }
  msg = util.format.apply(null, args);

  //
  // Respond to the callback.
  //
  function finish(err) {
    if (callback) {
      if (err) return callback(err);
      callback(null, level, msg, meta);
    }

    callback = null;
    if (!err) {
      self.emit('logged', level, msg, meta);
    }
  }

  // If we should pad for levels, do so
  if (this.padLevels) {
    msg = new Array(this.levelLength - level.length + 1).join(' ') + msg;
  }

  this.rewriters.forEach(function (rewriter) {
    meta = rewriter(level, msg, meta, self);
  });

  this.filters.forEach(function(filter) {
    var filtered = filter(level, msg, meta, self);
    if (typeof filtered === 'string')
      msg = filtered;
    else {
      msg = filtered.msg;
      meta = filtered.meta;
    }
  });

  //
  // For consideration of terminal 'color" programs like colors.js,
  // which can add ANSI escape color codes to strings, we destyle the
  // ANSI color escape codes when 'this.stripColors' is set.
  //
  // see: http://en.wikipedia.org/wiki/ANSI_escape_code
  //
  if (this.stripColors) {
    var code = /\u001b\[(\d+(;\d+)*)?m/g;
    msg = ('' + msg).replace(code, '');
  }

  //
  // Log for each transport and emit 'logging' event
  //
  function transportLog(name, next) {
    var transport = self.transports[name];
    transport.log(level, msg, meta, function (err) {
      if (err) {
        err.transport = transport;
        finish(err);
        return next();
      }

      self.emit('logging', transport, level, msg, meta);
      next();
    });
  }

  async.forEach(targets, transportLog, finish);
  return this;
}
```
- example usage
```shell
...

### Using the Default Logger
The default logger is accessible through the winston module directly. Any method that you could call on an instance of a logger
is available on the default logger:

''' js
  var winston = require('winston');

  winston.log('info', 'Hello distributed log files!');
  winston.info('Hello again distributed logs');

  winston.level = 'debug';
  winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:
...
```

#### <a name="apidoc.element.winston.Logger.prototype.profile"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>profile (id)](#apidoc.element.winston.Logger.prototype.profile)
- description and source-code
```javascript
profile = function (id) {
  var now = Date.now(), then, args,
      msg, meta, callback;

  if (this.profilers[id]) {
    then = this.profilers[id];
    delete this.profilers[id];

    // Support variable arguments: msg, meta, callback
    args     = Array.prototype.slice.call(arguments);
    callback = typeof args[args.length - 1] === 'function' ? args.pop() : null;
    meta     = typeof args[args.length - 1] === 'object' ? args.pop() : {};
    msg      = args.length === 2 ? args[1] : id;

    // Set the duration property of the metadata
    meta.durationMs = now - then;
    return this.info(msg, meta, callback);
  }
  else {
    this.profilers[id] = now;
  }

  return this;
}
```
- example usage
```shell
...
In addition to logging messages and metadata, winston also has a simple profiling mechanism implemented for any logger:

''' js
//
// Start profile of 'test'
// Remark: Consider using Date.now() with async operations
//
winston.profile('test');

setTimeout(function () {
  //
  // Stop profile of 'test'. Logging will now take place:
  //   "17 Jan 21:00:00 - info: test duration=1000ms"
  //
  winston.profile('test');
...
```

#### <a name="apidoc.element.winston.Logger.prototype.query"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>query (options, callback)](#apidoc.element.winston.Logger.prototype.query)
- description and source-code
```javascript
query = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }

  var self = this,
      options = options || {},
      results = {},
      query = common.clone(options.query) || {},
      transports;

  //
  // Helper function to query a single transport
  //
  function queryTransport(transport, next) {
    if (options.query) {
      options.query = transport.formatQuery(query);
    }

    transport.query(options, function (err, results) {
      if (err) {
        return next(err);
      }

      next(null, transport.formatResults(results, options.format));
    });
  }

  //
  // Helper function to accumulate the results from
  // 'queryTransport' into the 'results'.
  //
  function addResults(transport, next) {
    queryTransport(transport, function (err, result) {
      //
      // queryTransport could potentially invoke the callback
      // multiple times since Transport code can be unpredictable.
      //
      if (next) {
        result = err || result;
        if (result) {
          results[transport.name] = result;
        }

        next();
      }

      next = null;
    });
  }

  //
  // If an explicit transport is being queried then
  // respond with the results from only that transport
  //
  if (options.transport) {
    options.transport = options.transport.toLowerCase();
    return queryTransport(this.transports[options.transport], callback);
  }

  //
  // Create a list of all transports for this instance.
  //
  transports = this._names.map(function (name) {
    return self.transports[name];
  }).filter(function (transport) {
    return !!transport.query;
  });

  //
  // Iterate over the transports in parallel setting the
  // appropriate key in the 'results'
  //
  async.forEach(transports, addResults, function () {
    callback(null, results);
  });
}
```
- example usage
```shell
...
    order: 'desc',
    fields: ['message']
  };

  //
  // Find items logged between today and yesterday.
  //
  winston.query(options, function (err, results) {
    if (err) {
      throw err;
    }

    console.log(results);
  });
'''
...
```

#### <a name="apidoc.element.winston.Logger.prototype.remove"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>remove (transport)](#apidoc.element.winston.Logger.prototype.remove)
- description and source-code
```javascript
remove = function (transport) {
  var name = typeof transport !== 'string'
    ? transport.name || transport.prototype.name
    : transport;

  if (!this.transports[name]) {
    throw new Error('Transport ' + name + ' not attached to this instance');
  }

  var instance = this.transports[name];
  delete this.transports[name];
  this._names = Object.keys(this.transports);

  if (instance.close) {
    instance.close();
  }

  if (instance._onError) {
    instance.removeListener('error', instance._onError);
  }
  return this;
}
```
- example usage
```shell
...
winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:

''' js
winston.add(winston.transports.File, { filename: 'somefile.log' });
winston.remove(winston.transports.Console);
'''

Or do it with one call to configure():

''' js
winston.configure({
  transports: [
...
```

#### <a name="apidoc.element.winston.Logger.prototype.setLevels"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>setLevels (target)](#apidoc.element.winston.Logger.prototype.setLevels)
- description and source-code
```javascript
setLevels = function (target) {
  return common.setLevels(this, this.levels, target);
}
```
- example usage
```shell
...

As of 0.2.0, winston supports customizable logging levels, defaulting to [npm][0] style logging levels. Changing logging levels
is easy:

''' js
  //
  // Change levels on the default winston logger
  //
  winston.setLevels(winston.config.syslog.levels);

  //
  // Change levels on an instance of a logger
  //
  logger.setLevels(winston.config.syslog.levels);
'''
...
```

#### <a name="apidoc.element.winston.Logger.prototype.startTimer"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>startTimer ()](#apidoc.element.winston.Logger.prototype.startTimer)
- description and source-code
```javascript
startTimer = function () {
  return new ProfileHandler(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Logger.prototype.stream"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>stream (options)](#apidoc.element.winston.Logger.prototype.stream)
- description and source-code
```javascript
stream = function (options) {
  var self = this,
      options = options || {},
      out = new Stream,
      streams = [],
      transports;

  if (options.transport) {
    var transport = this.transports[options.transport];
    delete options.transport;
    if (transport && transport.stream) {
      return transport.stream(options);
    }
  }

  out._streams = streams;
  out.destroy = function () {
    var i = streams.length;
    while (i--) streams[i].destroy();
  };

  //
  // Create a list of all transports for this instance.
  //
  transports = this._names.map(function (name) {
    return self.transports[name];
  }).filter(function (transport) {
    return !!transport.stream;
  });

  transports.forEach(function (transport) {
    var stream = transport.stream(options);
    if (!stream) return;

    streams.push(stream);

    stream.on('log', function (log) {
      log.transport = log.transport || [];
      log.transport.push(transport.name);
      out.emit('log', log);
    });

    stream.on('error', function (err) {
      err.transport = err.transport || [];
      err.transport.push(transport.name);
      out.emit('error', err);
    });
  });

  return out;
}
```
- example usage
```shell
...
## Streaming Logs
Streaming allows you to stream your logs back from your chosen transport.

''' js
  //
  // Start at the end.
  //
  winston.stream({ start: -1 }).on('log', function(log) {
    console.log(log);
  });
'''

## Exceptions

### Handling Uncaught Exceptions with winston
...
```

#### <a name="apidoc.element.winston.Logger.prototype.unhandleExceptions"></a>[function <span class="apidocSignatureSpan">winston.Logger.prototype.</span>unhandleExceptions ()](#apidoc.element.winston.Logger.prototype.unhandleExceptions)
- description and source-code
```javascript
unhandleExceptions = function () {
  var self = this;

  if (this.catchExceptions) {
    Object.keys(this.exceptionHandlers).forEach(function (name) {
      var handler = self.exceptionHandlers[name];
      if (handler.close) {
        handler.close();
      }
    });

    this.exceptionHandlers = {};
    Object.keys(this.transports).forEach(function (name) {
      var transport = self.transports[name];
      if (transport.handleExceptions) {
        transport.handleExceptions = false;
      }
    })

    process.removeListener('uncaughtException', this.catchExceptions);
    this.catchExceptions = false;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.Transport"></a>[module winston.Transport](#apidoc.module.winston.Transport)

#### <a name="apidoc.element.winston.Transport.Transport"></a>[function <span class="apidocSignatureSpan">winston.</span>Transport (options)](#apidoc.element.winston.Transport.Transport)
- description and source-code
```javascript
Transport = function (options) {
  events.EventEmitter.call(this);

  options        = options        || {};
  this.silent    = options.silent || false;
  this.raw       = options.raw    || false;
  this.name      = options.name   || this.name;
  this.formatter = options.formatter;

  //
  // Do not set a default level. When 'level' is falsey on any
  // 'Transport' instance, any 'Logger' instance uses the
  // configured level (instead of the Transport level)
  //
  this.level = options.level;

  this.handleExceptions = options.handleExceptions || false;
  this.exceptionsLevel  = options.exceptionsLevel || 'error';
  this.humanReadableUnhandledException = options.humanReadableUnhandledException || false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Transport.super_"></a>[function <span class="apidocSignatureSpan">winston.Transport.</span>super_ ()](#apidoc.element.winston.Transport.super_)
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



# <a name="apidoc.module.winston.Transport.prototype"></a>[module winston.Transport.prototype](#apidoc.module.winston.Transport.prototype)

#### <a name="apidoc.element.winston.Transport.prototype.formatQuery"></a>[function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>formatQuery (query)](#apidoc.element.winston.Transport.prototype.formatQuery)
- description and source-code
```javascript
formatQuery = function (query) {
  return query;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Transport.prototype.formatResults"></a>[function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>formatResults (results, options)](#apidoc.element.winston.Transport.prototype.formatResults)
- description and source-code
```javascript
formatResults = function (results, options) {
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Transport.prototype.logException"></a>[function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>logException (msg, meta, callback)](#apidoc.element.winston.Transport.prototype.logException)
- description and source-code
```javascript
logException = function (msg, meta, callback) {
  var self = this,
      called;

  if (this.silent) {
    return callback();
  }

  function onComplete () {
    if (!called) {
      called = true;
      self.removeListener('logged', onComplete);
      self.removeListener('error', onComplete);
      callback();
    }
  }

  this.once('logged', onComplete);
  this.once('error', onComplete);
  this.log(self.exceptionsLevel, msg, meta, function () { });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.Transport.prototype.normalizeQuery"></a>[function <span class="apidocSignatureSpan">winston.Transport.prototype.</span>normalizeQuery (options)](#apidoc.element.winston.Transport.prototype.normalizeQuery)
- description and source-code
```javascript
normalizeQuery = function (options) {
  //
  // Use options similar to loggly.
  // [See Loggly Search API](http://wiki.loggly.com/retrieve_events#optional)
  //

  options = options || {};

  // limit
  options.rows = options.rows || options.limit || 10;

  // starting row offset
  options.start = options.start || 0;

  // now
  options.until = options.until || new Date;
  if (typeof options.until !== 'object') {
    options.until = new Date(options.until);
  }

  // now - 24
  options.from = options.from || (options.until - (24 * 60 * 60 * 1000));
  if (typeof options.from !== 'object') {
    options.from = new Date(options.from);
  }


  // 'asc' or 'desc'
  options.order = options.order || 'desc';

  // which fields to select
  options.fields = options.fields;

  return options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.config"></a>[module winston.config](#apidoc.module.winston.config)

#### <a name="apidoc.element.winston.config.addColors"></a>[function <span class="apidocSignatureSpan">winston.config.</span>addColors (colors)](#apidoc.element.winston.config.addColors)
- description and source-code
```javascript
addColors = function (colors) {
  mixin(allColors, colors);
}
```
- example usage
```shell
...

Although there is slight repetition in this data structure, it enables simple encapsulation if you do not want to have colors. If
 you do wish to have colors, in addition to passing the levels to the Logger itself, you must make winston aware of them:

''' js
  //
  // Make winston aware of these colors
  //
  winston.addColors(myCustomLevels.colors);
'''

This enables transports with the 'colorize' option set to appropriately color the output of custom levels.

## Further Reading

### Events and Callbacks in Winston
...
```

#### <a name="apidoc.element.winston.config.colorize"></a>[function <span class="apidocSignatureSpan">winston.config.</span>colorize (level, message)](#apidoc.element.winston.config.colorize)
- description and source-code
```javascript
colorize = function (level, message) {
  if (typeof message === 'undefined') message = level;

  var colorized = message;
  if (allColors[level] instanceof Array) {
    for (var i = 0, l = allColors[level].length; i < l; ++i) {
      colorized = colors[allColors[level][i]](colorized);
    }
  }
  else if (allColors[level].match(/\s/)) {
    var colorArr = allColors[level].split(/\s+/);
    for (var i = 0; i < colorArr.length; ++i) {
      colorized = colors[colorArr[i]](colorized);
    }
    allColors[level] = colorArr;
  }
  else {
    colorized = colors[allColors[level]](colorized);
  }

  return colorized;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.exception"></a>[module winston.exception](#apidoc.module.winston.exception)

#### <a name="apidoc.element.winston.exception.getAllInfo"></a>[function <span class="apidocSignatureSpan">winston.exception.</span>getAllInfo (err)](#apidoc.element.winston.exception.getAllInfo)
- description and source-code
```javascript
getAllInfo = function (err) {
  return {
    date:    new Date().toString(),
    process: exception.getProcessInfo(),
    os:      exception.getOsInfo(),
    trace:   exception.getTrace(err),
    stack:   err.stack && err.stack.split('\n')
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.exception.getOsInfo"></a>[function <span class="apidocSignatureSpan">winston.exception.</span>getOsInfo ()](#apidoc.element.winston.exception.getOsInfo)
- description and source-code
```javascript
getOsInfo = function () {
  return {
    loadavg: os.loadavg(),
    uptime:  os.uptime()
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.exception.getProcessInfo"></a>[function <span class="apidocSignatureSpan">winston.exception.</span>getProcessInfo ()](#apidoc.element.winston.exception.getProcessInfo)
- description and source-code
```javascript
getProcessInfo = function () {
  return {
    pid:         process.pid,
    uid:         process.getuid ? process.getuid() : null,
    gid:         process.getgid ? process.getgid() : null,
    cwd:         process.cwd(),
    execPath:    process.execPath,
    version:     process.version,
    argv:        process.argv,
    memoryUsage: process.memoryUsage()
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.exception.getTrace"></a>[function <span class="apidocSignatureSpan">winston.exception.</span>getTrace (err)](#apidoc.element.winston.exception.getTrace)
- description and source-code
```javascript
getTrace = function (err) {
  var trace = err ? stackTrace.parse(err) : stackTrace.get();
  return trace.map(function (site) {
    return {
      column:   site.getColumnNumber(),
      file:     site.getFileName(),
      function: site.getFunctionName(),
      line:     site.getLineNumber(),
      method:   site.getMethodName(),
      native:   site.isNative(),
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.transports"></a>[module winston.transports](#apidoc.module.winston.transports)

#### <a name="apidoc.element.winston.transports.Console"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>Console (options)](#apidoc.element.winston.transports.Console)
- description and source-code
```javascript
Console = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.json         = options.json        || false;
  this.colorize     = options.colorize    || false;
  this.prettyPrint  = options.prettyPrint || false;
  this.timestamp    = typeof options.timestamp !== 'undefined' ? options.timestamp : false;
  this.showLevel    = options.showLevel === undefined ? true : options.showLevel;
  this.label        = options.label       || null;
  this.logstash     = options.logstash    || false;
  this.depth        = options.depth       || null;
  this.align        = options.align       || false;
  this.stderrLevels = setStderrLevels(options.stderrLevels, options.debugStdout);
  this.eol          = options.eol   || os.EOL;

  if (this.json) {
    this.stringify = options.stringify || function (obj) {
      return JSON.stringify(obj, null, 2);
    };
  }

  //
  // Convert stderrLevels into an Object for faster key-lookup times than an Array.
  //
  // For backwards compatibility, stderrLevels defaults to ['error', 'debug']
  // or ['error'] depending on whether options.debugStdout is true.
  //
  function setStderrLevels (levels, debugStdout) {
    var defaultMsg = 'Cannot have non-string elements in stderrLevels Array';
    if (debugStdout) {
      if (levels) {
        //
        // Don't allow setting both debugStdout and stderrLevels together,
        // since this could cause behaviour a programmer might not expect.
        //
        throw new Error('Cannot set debugStdout and stderrLevels together');
      }

      return common.stringArrayToSet(['error'], defaultMsg);
    }

    if (!levels) {
      return common.stringArrayToSet(['error', 'debug'], defaultMsg);
    } else if (!(Array.isArray(levels))) {
      throw new Error('Cannot set stderrLevels to type other than Array');
    }

    return common.stringArrayToSet(levels, defaultMsg);
  };
}
```
- example usage
```shell
...
'''

Example 2

''' js
var logger = new winston.Logger({
  transports: [
    new winston.transports.Console({
      handleExceptions: true,
      json: true
    })
  ],
  exitOnError: false
});
'''
...
```

#### <a name="apidoc.element.winston.transports.File"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>File (options)](#apidoc.element.winston.transports.File)
- description and source-code
```javascript
File = function (options) {
  var self = this;
  Transport.call(this, options);

  //
  // Helper function which throws an 'Error' in the event
  // that any of the rest of the arguments is present in 'options'.
  //
  function throwIf (target /*, illegal... */) {
    Array.prototype.slice.call(arguments, 1).forEach(function (name) {
      if (options[name]) {
        throw new Error('Cannot set ' + name + ' and ' + target + 'together');
      }
    });
  }

  if (options.filename || options.dirname) {
    throwIf('filename or dirname', 'stream');
    this._basename = this.filename = options.filename
      ? path.basename(options.filename)
      : 'winston.log';

    this.dirname = options.dirname || path.dirname(options.filename);
    this.options = options.options || { flags: 'a' };

    //
    // "24 bytes" is maybe a good value for logging lines.
    //
    this.options.highWaterMark = this.options.highWaterMark || 24;
  }
  else if (options.stream) {
    throwIf('stream', 'filename', 'maxsize');
    this._stream = options.stream;
    this._isStreams2 = isWritable(this._stream);
    this._stream.on('error', function(error){
      self.emit('error', error);
    });
    //
    // We need to listen for drain events when
    // write() returns false. This can make node
    // mad at times.
    //
    this._stream.setMaxListeners(Infinity);
  }
  else {
    throw new Error('Cannot log to file without filename or stream.');
  }

  this.json        = options.json !== false;
  this.logstash    = options.logstash    || false;
  this.colorize    = options.colorize    || false;
  this.maxsize     = options.maxsize     || null;
  this.rotationFormat = options.rotationFormat || false;
  this.zippedArchive = options.zippedArchive || false;
  this.maxFiles    = options.maxFiles    || null;
  this.prettyPrint = options.prettyPrint || false;
  this.label       = options.label       || null;
  this.timestamp   = options.timestamp != null ? options.timestamp : true;
  this.eol         = options.eol || os.EOL;
  this.tailable    = options.tailable    || false;
  this.depth       = options.depth       || null;
  this.showLevel   = options.showLevel === undefined ? true : options.showLevel;
  this.maxRetries  = options.maxRetries || 2;

  if (this.json) {
    this.stringify = options.stringify;
  }

  //
  // Internal state variables representing the number
  // of files this instance has created and the current
  // size (in bytes) of the current logfile.
  //
  this._size     = 0;
  this._created  = 0;
  this._buffer   = [];
  this._draining = false;
  this._opening  = false;
  this._failures = 0;
  this._archive = null;
}
```
- example usage
```shell
...

If you want to use this feature with the default logger simply call '.handleExceptions()' with a transport instance.

''' js
//
// You can add a separate exception logger by passing it to '.handleExceptions'
//
winston.handleExceptions(new winston.transports.File({ filename: 'path/to/exceptions.log' }))

//
// Alternatively you can set '.handleExceptions' to true when adding transports to winston.
// You can use the '.humanReadableUnhandledException' option to get more readable exceptions.
//
winston.add(winston.transports.File, {
  filename: 'path/to/all-logs.log',
...
```

#### <a name="apidoc.element.winston.transports.Http"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>Http (options)](#apidoc.element.winston.transports.Http)
- description and source-code
```javascript
Http = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.name = 'http';
  this.ssl = !!options.ssl;
  this.host = options.host || 'localhost';
  this.port = options.port;
  this.auth = options.auth;
  this.path = options.path || '';
  this.agent = options.agent;

  if (!this.port) {
    this.port = this.ssl ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.Memory"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>Memory (options)](#apidoc.element.winston.transports.Memory)
- description and source-code
```javascript
Memory = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.errorOutput = [];
  this.writeOutput = [];

  this.json        = options.json        || false;
  this.colorize    = options.colorize    || false;
  this.prettyPrint = options.prettyPrint || false;
  this.timestamp   = typeof options.timestamp !== 'undefined' ? options.timestamp : false;
  this.showLevel   = options.showLevel === undefined ? true : options.showLevel;
  this.label       = options.label       || null;
  this.depth       = options.depth       || null;

  if (this.json) {
    this.stringify = options.stringify || function (obj) {
      return JSON.stringify(obj, null, 2);
    };
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.transports.Console"></a>[module winston.transports.Console](#apidoc.module.winston.transports.Console)

#### <a name="apidoc.element.winston.transports.Console.Console"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>Console (options)](#apidoc.element.winston.transports.Console.Console)
- description and source-code
```javascript
Console = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.json         = options.json        || false;
  this.colorize     = options.colorize    || false;
  this.prettyPrint  = options.prettyPrint || false;
  this.timestamp    = typeof options.timestamp !== 'undefined' ? options.timestamp : false;
  this.showLevel    = options.showLevel === undefined ? true : options.showLevel;
  this.label        = options.label       || null;
  this.logstash     = options.logstash    || false;
  this.depth        = options.depth       || null;
  this.align        = options.align       || false;
  this.stderrLevels = setStderrLevels(options.stderrLevels, options.debugStdout);
  this.eol          = options.eol   || os.EOL;

  if (this.json) {
    this.stringify = options.stringify || function (obj) {
      return JSON.stringify(obj, null, 2);
    };
  }

  //
  // Convert stderrLevels into an Object for faster key-lookup times than an Array.
  //
  // For backwards compatibility, stderrLevels defaults to ['error', 'debug']
  // or ['error'] depending on whether options.debugStdout is true.
  //
  function setStderrLevels (levels, debugStdout) {
    var defaultMsg = 'Cannot have non-string elements in stderrLevels Array';
    if (debugStdout) {
      if (levels) {
        //
        // Don't allow setting both debugStdout and stderrLevels together,
        // since this could cause behaviour a programmer might not expect.
        //
        throw new Error('Cannot set debugStdout and stderrLevels together');
      }

      return common.stringArrayToSet(['error'], defaultMsg);
    }

    if (!levels) {
      return common.stringArrayToSet(['error', 'debug'], defaultMsg);
    } else if (!(Array.isArray(levels))) {
      throw new Error('Cannot set stderrLevels to type other than Array');
    }

    return common.stringArrayToSet(levels, defaultMsg);
  };
}
```
- example usage
```shell
...
'''

Example 2

''' js
var logger = new winston.Logger({
  transports: [
    new winston.transports.Console({
      handleExceptions: true,
      json: true
    })
  ],
  exitOnError: false
});
'''
...
```

#### <a name="apidoc.element.winston.transports.Console.super_"></a>[function <span class="apidocSignatureSpan">winston.transports.Console.</span>super_ (options)](#apidoc.element.winston.transports.Console.super_)
- description and source-code
```javascript
super_ = function (options) {
  events.EventEmitter.call(this);

  options        = options        || {};
  this.silent    = options.silent || false;
  this.raw       = options.raw    || false;
  this.name      = options.name   || this.name;
  this.formatter = options.formatter;

  //
  // Do not set a default level. When 'level' is falsey on any
  // 'Transport' instance, any 'Logger' instance uses the
  // configured level (instead of the Transport level)
  //
  this.level = options.level;

  this.handleExceptions = options.handleExceptions || false;
  this.exceptionsLevel  = options.exceptionsLevel || 'error';
  this.humanReadableUnhandledException = options.humanReadableUnhandledException || false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.transports.Console.prototype"></a>[module winston.transports.Console.prototype](#apidoc.module.winston.transports.Console.prototype)

#### <a name="apidoc.element.winston.transports.Console.prototype.log"></a>[function <span class="apidocSignatureSpan">winston.transports.Console.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.Console.prototype.log)
- description and source-code
```javascript
log = function (level, msg, meta, callback) {
  if (this.silent) {
    return callback(null, true);
  }

  var self = this,
      output;

  output = common.log({
    colorize:    this.colorize,
    json:        this.json,
    level:       level,
    message:     msg,
    meta:        meta,
    stringify:   this.stringify,
    timestamp:   this.timestamp,
    showLevel:   this.showLevel,
    prettyPrint: this.prettyPrint,
    raw:         this.raw,
    label:       this.label,
    logstash:    this.logstash,
    depth:       this.depth,
    formatter:   this.formatter,
    align:       this.align,
    humanReadableUnhandledException: this.humanReadableUnhandledException
  });

  if (this.stderrLevels[level]) {
    process.stderr.write(output + this.eol);
  } else {
    process.stdout.write(output + this.eol);
  }

  //
  // Emit the 'logged' event immediately because the event loop
  // will not exit until 'process.stdout' has drained anyway.
  //
  self.emit('logged');
  callback(null, true);
}
```
- example usage
```shell
...

### Using the Default Logger
The default logger is accessible through the winston module directly. Any method that you could call on an instance of a logger
is available on the default logger:

''' js
  var winston = require('winston');

  winston.log('info', 'Hello distributed log files!');
  winston.info('Hello again distributed logs');

  winston.level = 'debug';
  winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:
...
```



# <a name="apidoc.module.winston.transports.File"></a>[module winston.transports.File](#apidoc.module.winston.transports.File)

#### <a name="apidoc.element.winston.transports.File.File"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>File (options)](#apidoc.element.winston.transports.File.File)
- description and source-code
```javascript
File = function (options) {
  var self = this;
  Transport.call(this, options);

  //
  // Helper function which throws an 'Error' in the event
  // that any of the rest of the arguments is present in 'options'.
  //
  function throwIf (target /*, illegal... */) {
    Array.prototype.slice.call(arguments, 1).forEach(function (name) {
      if (options[name]) {
        throw new Error('Cannot set ' + name + ' and ' + target + 'together');
      }
    });
  }

  if (options.filename || options.dirname) {
    throwIf('filename or dirname', 'stream');
    this._basename = this.filename = options.filename
      ? path.basename(options.filename)
      : 'winston.log';

    this.dirname = options.dirname || path.dirname(options.filename);
    this.options = options.options || { flags: 'a' };

    //
    // "24 bytes" is maybe a good value for logging lines.
    //
    this.options.highWaterMark = this.options.highWaterMark || 24;
  }
  else if (options.stream) {
    throwIf('stream', 'filename', 'maxsize');
    this._stream = options.stream;
    this._isStreams2 = isWritable(this._stream);
    this._stream.on('error', function(error){
      self.emit('error', error);
    });
    //
    // We need to listen for drain events when
    // write() returns false. This can make node
    // mad at times.
    //
    this._stream.setMaxListeners(Infinity);
  }
  else {
    throw new Error('Cannot log to file without filename or stream.');
  }

  this.json        = options.json !== false;
  this.logstash    = options.logstash    || false;
  this.colorize    = options.colorize    || false;
  this.maxsize     = options.maxsize     || null;
  this.rotationFormat = options.rotationFormat || false;
  this.zippedArchive = options.zippedArchive || false;
  this.maxFiles    = options.maxFiles    || null;
  this.prettyPrint = options.prettyPrint || false;
  this.label       = options.label       || null;
  this.timestamp   = options.timestamp != null ? options.timestamp : true;
  this.eol         = options.eol || os.EOL;
  this.tailable    = options.tailable    || false;
  this.depth       = options.depth       || null;
  this.showLevel   = options.showLevel === undefined ? true : options.showLevel;
  this.maxRetries  = options.maxRetries || 2;

  if (this.json) {
    this.stringify = options.stringify;
  }

  //
  // Internal state variables representing the number
  // of files this instance has created and the current
  // size (in bytes) of the current logfile.
  //
  this._size     = 0;
  this._created  = 0;
  this._buffer   = [];
  this._draining = false;
  this._opening  = false;
  this._failures = 0;
  this._archive = null;
}
```
- example usage
```shell
...

If you want to use this feature with the default logger simply call '.handleExceptions()' with a transport instance.

''' js
//
// You can add a separate exception logger by passing it to '.handleExceptions'
//
winston.handleExceptions(new winston.transports.File({ filename: 'path/to/exceptions.log' }))

//
// Alternatively you can set '.handleExceptions' to true when adding transports to winston.
// You can use the '.humanReadableUnhandledException' option to get more readable exceptions.
//
winston.add(winston.transports.File, {
  filename: 'path/to/all-logs.log',
...
```

#### <a name="apidoc.element.winston.transports.File.super_"></a>[function <span class="apidocSignatureSpan">winston.transports.File.</span>super_ (options)](#apidoc.element.winston.transports.File.super_)
- description and source-code
```javascript
super_ = function (options) {
  events.EventEmitter.call(this);

  options        = options        || {};
  this.silent    = options.silent || false;
  this.raw       = options.raw    || false;
  this.name      = options.name   || this.name;
  this.formatter = options.formatter;

  //
  // Do not set a default level. When 'level' is falsey on any
  // 'Transport' instance, any 'Logger' instance uses the
  // configured level (instead of the Transport level)
  //
  this.level = options.level;

  this.handleExceptions = options.handleExceptions || false;
  this.exceptionsLevel  = options.exceptionsLevel || 'error';
  this.humanReadableUnhandledException = options.humanReadableUnhandledException || false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.transports.File.prototype"></a>[module winston.transports.File.prototype](#apidoc.module.winston.transports.File.prototype)

#### <a name="apidoc.element.winston.transports.File.prototype._checkMaxFilesIncrementing"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_checkMaxFilesIncrementing (ext, basename, callback)](#apidoc.element.winston.transports.File.prototype._checkMaxFilesIncrementing)
- description and source-code
```javascript
_checkMaxFilesIncrementing = function (ext, basename, callback) {
  var oldest, target,
    self = this;

  if (self.zippedArchive) {
    self._archive = path.join(self.dirname, basename +
        ((self._created === 1) ? '' : self._created-1) +
        ext);
  }


  // Check for maxFiles option and delete file
  if (!self.maxFiles || self._created < self.maxFiles) {
    return callback();
  }

  oldest = self._created - self.maxFiles;
  target = path.join(self.dirname, basename + (oldest !== 0 ? oldest : '') + ext +
    (self.zippedArchive ? '.gz' : ''));
  fs.unlink(target, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype._checkMaxFilesTailable"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_checkMaxFilesTailable (ext, basename, callback)](#apidoc.element.winston.transports.File.prototype._checkMaxFilesTailable)
- description and source-code
```javascript
_checkMaxFilesTailable = function (ext, basename, callback) {
  var tasks = [],
      self = this;

  if (!this.maxFiles)
    return;

  for (var x = this.maxFiles - 1; x > 0; x--) {
    tasks.push(function (i) {
      return function (cb) {
        var tmppath = path.join(self.dirname, basename + (i - 1) + ext +
          (self.zippedArchive ? '.gz' : ''));
        fs.exists(tmppath, function (exists) {
          if (!exists) {
            return cb(null);
          }

          fs.rename(tmppath, path.join(self.dirname, basename + i + ext +
            (self.zippedArchive ? '.gz' : '')), cb);
        });
      };
    }(x));
  }

  if (self.zippedArchive) {
    self._archive = path.join(self.dirname, basename + 1 + ext);
  }
  async.series(tasks, function (err) {
    fs.rename(
      path.join(self.dirname, basename + ext),
      path.join(self.dirname, basename + 1 + ext),
      callback
    );
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype._createStream"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_createStream ()](#apidoc.element.winston.transports.File.prototype._createStream)
- description and source-code
```javascript
_createStream = function () {
  var self = this;
  this.opening = true;

  (function checkFile (target) {
    var fullname = path.join(self.dirname, target);

    //
    // Creates the 'WriteStream' and then flushes any
    // buffered messages.
    //
    function createAndFlush (size) {
      if (self._stream) {
        self._stream.end();
        self._stream.destroySoon();
      }

      self._size = size;
      self.filename = target;
      self._stream = fs.createWriteStream(fullname, self.options);
      self._isStreams2 = isWritable(self._stream);
      self._stream.on('error', function(error){
        if (self._failures < self.maxRetries) {
          self._createStream();
          self._failures++;
        }
        else {
          self.emit('error', error);
        }
      });
      //
      // We need to listen for drain events when
      // write() returns false. This can make node
      // mad at times.
      //
      self._stream.setMaxListeners(Infinity);

      //
      // When the current stream has finished flushing
      // then we can be sure we have finished opening
      // and thus can emit the 'open' event.
      //
      self.once('flush', function () {
        // Because "flush" event is based on native stream "drain" event,
        // logs could be written inbetween "self.flush()" and here
        // Therefore, we need to flush again to make sure everything is flushed
        self.flush();

        self.opening = false;
        self.emit('open', fullname);
      });
      //
      // Remark: It is possible that in the time it has taken to find the
      // next logfile to be written more data than 'maxsize' has been buffered,
      // but for sensible limits (10s - 100s of MB) this seems unlikely in less
      // than one second.
      //
      self.flush();
      compressFile();
    }

    function compressFile() {
      if (self._archive) {
        var gzip = zlib.createGzip();

        var inp = fs.createReadStream(String(self._archive));
        var out = fs.createWriteStream(self._archive + '.gz');

        inp.pipe(gzip).pipe(out);

        fs.unlink(String(self._archive));
        self._archive = '';
      }
    }

    fs.stat(fullname, function (err, stats) {
      if (err) {
        if (err.code !== 'ENOENT') {
          return self.emit('error', err);
        }
        return createAndFlush(0);
      }

      if (!stats || (self.maxsize && stats.size >= self.maxsize)) {
        //
        // If 'stats.size' is greater than the 'maxsize' for
        // this instance then try again
        //
        return self._incFile(function() {
          checkFile(self._getFile());
        });
      }

      createAndFlush(stats.size);
    });
  })(this._getFile());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype._getFile"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_getFile ()](#apidoc.element.winston.transports.File.prototype._getFile)
- description and source-code
```javascript
_getFile = function () {
  var ext = path.extname(this._basename),
      basename = path.basename(this._basename, ext);

  //
  // Caveat emptor (indexzero): rotationFormat() was broken by design
  // when combined with max files because the set of files to unlink
  // is never stored.
  //
  return !this.tailable && this._created
    ? basename + (this.rotationFormat ? this.rotationFormat() : this._created) + ext
    : basename + ext;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype._incFile"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_incFile (callback)](#apidoc.element.winston.transports.File.prototype._incFile)
- description and source-code
```javascript
_incFile = function (callback) {
  var ext = path.extname(this._basename),
      basename = path.basename(this._basename, ext),
      oldest,
      target;

  if (!this.tailable) {
    this._created += 1;
    this._checkMaxFilesIncrementing(ext, basename, callback);
  }
  else {
    this._checkMaxFilesTailable(ext, basename, callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype._lazyDrain"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_lazyDrain ()](#apidoc.element.winston.transports.File.prototype._lazyDrain)
- description and source-code
```javascript
_lazyDrain = function () {
  var self = this;

  if (!this._draining && this._stream) {
    this._draining = true;

    this._stream.once('drain', function () {
      this._draining = false;
      self.emit('logged');
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype._write"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>_write (data, callback)](#apidoc.element.winston.transports.File.prototype._write)
- description and source-code
```javascript
_write = function (data, callback) {
  if (this._isStreams2) {
    this._stream.write(data);
    return callback && process.nextTick(function () {
      callback(null, true);
    });
  }

  // If this is a file write stream, we could use the builtin
  // callback functionality, however, the stream is not guaranteed
  // to be an fs.WriteStream.
  var ret = this._stream.write(data);
  if (!callback) return;
  if (ret === false) {
    return this._stream.once('drain', function() {
      callback(null, true);
    });
  }
  process.nextTick(function () {
    callback(null, true);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype.close"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>close ()](#apidoc.element.winston.transports.File.prototype.close)
- description and source-code
```javascript
close = function () {
  var self = this;

  if (this._stream) {
    this._stream.end();
    this._stream.destroySoon();

    this._stream.once('finish', function () {
      self.emit('flush');
      self.emit('closed');
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype.flush"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>flush ()](#apidoc.element.winston.transports.File.prototype.flush)
- description and source-code
```javascript
flush = function () {
  var self = this;

  // If nothing to flush, there will be no "flush" event from native stream
  // Thus, the "open" event will never be fired (see _createStream.createAndFlush function)
  // That means, self.opening will never set to false and no logs will be written to disk
  if (!this._buffer.length) {
    return self.emit('flush');
  }

  //
  // Iterate over the '_buffer' of enqueued messaged
  // and then write them to the newly created stream.
  //
  this._buffer.forEach(function (item) {
    var str = item[0],
        callback = item[1];

    process.nextTick(function () {
      self._write(str, callback);
      self._size += str.length;
    });
  });

  //
  // Quickly truncate the '_buffer' once the write operations
  // have been started
  //
  self._buffer.length = 0;

  //
  // When the stream has drained we have flushed
  // our buffer.
  //
  self._stream.once('drain', function () {
    self.emit('flush');
    self.emit('logged');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype.log"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.File.prototype.log)
- description and source-code
```javascript
log = function (level, msg, meta, callback) {
  if (this.silent) {
    return callback(null, true);
  }

  //
  // If failures exceeds maxRetries then we can't access the
  // stream. In this case we need to perform a noop and return
  // an error.
  //
  if (this._failures >= this.maxRetries) {
    return callback(new Error('Transport is in a failed state.'));
  }

  var self = this;

  if (typeof msg !== 'string') {
    msg = '' + msg;
  }

  var output = common.log({
    level:       level,
    message:     msg,
    meta:        meta,
    json:        this.json,
    logstash:    this.logstash,
    colorize:    this.colorize,
    prettyPrint: this.prettyPrint,
    timestamp:   this.timestamp,
    showLevel:   this.showLevel,
    stringify:   this.stringify,
    label:       this.label,
    depth:       this.depth,
    formatter:   this.formatter,
    humanReadableUnhandledException: this.humanReadableUnhandledException
  });

  if (typeof output === 'string') {
    output += this.eol;
  }

  if (!this.filename) {
    //
    // If there is no 'filename' on this instance then it was configured
    // with a raw 'WriteableStream' instance and we should not perform any
    // size restrictions.
    //
    this._write(output, callback);
    this._size += output.length;
    this._lazyDrain();
  }
  else {
    this.open(function (err) {
      if (err) {
        //
        // If there was an error enqueue the message
        //
        return self._buffer.push([output, callback]);
      }

      self._write(output, callback);
      self._size += output.length;
      self._lazyDrain();
    });
  }
}
```
- example usage
```shell
...

### Using the Default Logger
The default logger is accessible through the winston module directly. Any method that you could call on an instance of a logger
is available on the default logger:

''' js
  var winston = require('winston');

  winston.log('info', 'Hello distributed log files!');
  winston.info('Hello again distributed logs');

  winston.level = 'debug';
  winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:
...
```

#### <a name="apidoc.element.winston.transports.File.prototype.open"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>open (callback)](#apidoc.element.winston.transports.File.prototype.open)
- description and source-code
```javascript
open = function (callback) {
  if (this.opening) {
    //
    // If we are already attempting to open the next
    // available file then respond with a value indicating
    // that the message should be buffered.
    //
    return callback(true);
  }
  else if (!this._stream || (this.maxsize && this._size >= this.maxsize)) {
    //
    // If we dont have a stream or have exceeded our size, then create
    // the next stream and respond with a value indicating that
    // the message should be buffered.
    //
    callback(true);
    return this._createStream();
  }

  this._archive = this.zippedArchive ? this._stream.path : null;

  //
  // Otherwise we have a valid (and ready) stream.
  //
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.File.prototype.query"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>query (options, callback)](#apidoc.element.winston.transports.File.prototype.query)
- description and source-code
```javascript
query = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }

  var file = path.join(this.dirname, this.filename),
      options = this.normalizeQuery(options),
      buff = '',
      results = [],
      row = 0;

  var stream = fs.createReadStream(file, {
    encoding: 'utf8'
  });

  stream.on('error', function (err) {
    if (stream.readable) {
      stream.destroy();
    }
    if (!callback) return;
    return err.code !== 'ENOENT'
      ? callback(err)
      : callback(null, results);
  });

  stream.on('data', function (data) {
    var data = (buff + data).split(/\n+/),
        l = data.length - 1,
        i = 0;

    for (; i < l; i++) {
      if (!options.start || row >= options.start) {
        add(data[i]);
      }
      row++;
    }

    buff = data[l];
  });

  stream.on('close', function () {
    if (buff) add(buff, true);
    if (options.order === 'desc') {
      results = results.reverse();
    }
    if (callback) callback(null, results);
  });

  function add(buff, attempt) {
    try {
      var log = JSON.parse(buff);
      if (check(log)) push(log);
    } catch (e) {
      if (!attempt) {
        stream.emit('error', e);
      }
    }
  }

  function push(log) {
    if (options.rows && results.length >= options.rows
        && options.order != 'desc') {
      if (stream.readable) {
        stream.destroy();
      }
      return;
    }

    if (options.fields) {
      var obj = {};
      options.fields.forEach(function (key) {
        obj[key] = log[key];
      });
      log = obj;
    }

    if (options.order === 'desc') {
      if (results.length >= options.rows) {
        results.shift();
      }
    }
    results.push(log);
  }

  function check(log) {
    if (!log) return;

    if (typeof log !== 'object') return;

    var time = new Date(log.timestamp);
    if ((options.from && time < options.from)
        || (options.until && time > options.until)) {
      return;
    }

    return true;
  }
}
```
- example usage
```shell
...
    order: 'desc',
    fields: ['message']
  };

  //
  // Find items logged between today and yesterday.
  //
  winston.query(options, function (err, results) {
    if (err) {
      throw err;
    }

    console.log(results);
  });
'''
...
```

#### <a name="apidoc.element.winston.transports.File.prototype.stream"></a>[function <span class="apidocSignatureSpan">winston.transports.File.prototype.</span>stream (options)](#apidoc.element.winston.transports.File.prototype.stream)
- description and source-code
```javascript
stream = function (options) {
  var file = path.join(this.dirname, this.filename),
      options = options || {},
      stream = new Stream;

  var tail = {
    file: file,
    start: options.start
  };

  stream.destroy = common.tailFile(tail, function (err, line) {

    if(err){
      return stream.emit('error',err);
    }

    try {
      stream.emit('data', line);
      line = JSON.parse(line);
      stream.emit('log', line);
    } catch (e) {
      stream.emit('error', e);
    }
  });

  return stream;
}
```
- example usage
```shell
...
## Streaming Logs
Streaming allows you to stream your logs back from your chosen transport.

''' js
  //
  // Start at the end.
  //
  winston.stream({ start: -1 }).on('log', function(log) {
    console.log(log);
  });
'''

## Exceptions

### Handling Uncaught Exceptions with winston
...
```



# <a name="apidoc.module.winston.transports.Http"></a>[module winston.transports.Http](#apidoc.module.winston.transports.Http)

#### <a name="apidoc.element.winston.transports.Http.Http"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>Http (options)](#apidoc.element.winston.transports.Http.Http)
- description and source-code
```javascript
Http = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.name = 'http';
  this.ssl = !!options.ssl;
  this.host = options.host || 'localhost';
  this.port = options.port;
  this.auth = options.auth;
  this.path = options.path || '';
  this.agent = options.agent;

  if (!this.port) {
    this.port = this.ssl ? 443 : 80;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.Http.super_"></a>[function <span class="apidocSignatureSpan">winston.transports.Http.</span>super_ (options)](#apidoc.element.winston.transports.Http.super_)
- description and source-code
```javascript
super_ = function (options) {
  events.EventEmitter.call(this);

  options        = options        || {};
  this.silent    = options.silent || false;
  this.raw       = options.raw    || false;
  this.name      = options.name   || this.name;
  this.formatter = options.formatter;

  //
  // Do not set a default level. When 'level' is falsey on any
  // 'Transport' instance, any 'Logger' instance uses the
  // configured level (instead of the Transport level)
  //
  this.level = options.level;

  this.handleExceptions = options.handleExceptions || false;
  this.exceptionsLevel  = options.exceptionsLevel || 'error';
  this.humanReadableUnhandledException = options.humanReadableUnhandledException || false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.transports.Http.prototype"></a>[module winston.transports.Http.prototype](#apidoc.module.winston.transports.Http.prototype)

#### <a name="apidoc.element.winston.transports.Http.prototype._request"></a>[function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>_request (options, callback)](#apidoc.element.winston.transports.Http.prototype._request)
- description and source-code
```javascript
_request = function (options, callback) {
  options = options || {};

  var auth = options.auth || this.auth,
      path = options.path || this.path || '',
      req;

  delete options.auth;
  delete options.path;

  // Prepare options for outgoing HTTP request
  req = (this.ssl ? https : http).request({
    host: this.host,
    port: this.port,
    path: '/' + path.replace(/^\//, ''),
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    agent: this.agent,
    auth: (auth) ? auth.username + ':' + auth.password : ''
  });

  req.on('error', callback);
  req.on('response', function (res) {
    var body = '';

    res.on('data', function (chunk) {
      body += chunk;
    });

    res.on('end', function () {
      callback(null, res, body);
    });

    res.resume();
  });

  req.end(new Buffer(JSON.stringify(options), 'utf8'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.Http.prototype.log"></a>[function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.Http.prototype.log)
- description and source-code
```javascript
log = function (level, msg, meta, callback) {
  var self = this;

  if (typeof meta === 'function') {
    callback = meta;
    meta = {};
  }

  var options = {
    method: 'collect',
    params: {
      level: level,
      message: msg,
      meta: meta
    }
  };

  if (meta) {
    if (meta.path) {
      options.path = meta.path;
      delete meta.path;
    }

    if (meta.auth) {
      options.auth = meta.auth;
      delete meta.auth;
    }
  }

  this._request(options, function (err, res) {
    if (res && res.statusCode !== 200) {
      err = new Error('HTTP Status Code: ' + res.statusCode);
    }

    if (err) return callback(err);

    // TODO: emit 'logged' correctly,
    // keep track of pending logs.
    self.emit('logged');

    if (callback) callback(null, true);
  });
}
```
- example usage
```shell
...

### Using the Default Logger
The default logger is accessible through the winston module directly. Any method that you could call on an instance of a logger
is available on the default logger:

''' js
  var winston = require('winston');

  winston.log('info', 'Hello distributed log files!');
  winston.info('Hello again distributed logs');

  winston.level = 'debug';
  winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:
...
```

#### <a name="apidoc.element.winston.transports.Http.prototype.query"></a>[function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>query (options, callback)](#apidoc.element.winston.transports.Http.prototype.query)
- description and source-code
```javascript
query = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }

  var self = this,
      options = this.normalizeQuery(options);

  options = {
    method: 'query',
    params: options
  };

  if (options.params.path) {
    options.path = options.params.path;
    delete options.params.path;
  }

  if (options.params.auth) {
    options.auth = options.params.auth;
    delete options.params.auth;
  }

  this._request(options, function (err, res, body) {
    if (res && res.statusCode !== 200) {
      err = new Error('HTTP Status Code: ' + res.statusCode);
    }

    if (err) return callback(err);

    if (typeof body === 'string') {
      try {
        body = JSON.parse(body);
      } catch (e) {
        return callback(e);
      }
    }

    callback(null, body);
  });
}
```
- example usage
```shell
...
    order: 'desc',
    fields: ['message']
  };

  //
  // Find items logged between today and yesterday.
  //
  winston.query(options, function (err, results) {
    if (err) {
      throw err;
    }

    console.log(results);
  });
'''
...
```

#### <a name="apidoc.element.winston.transports.Http.prototype.stream"></a>[function <span class="apidocSignatureSpan">winston.transports.Http.prototype.</span>stream (options)](#apidoc.element.winston.transports.Http.prototype.stream)
- description and source-code
```javascript
stream = function (options) {
  options = options || {};

  var self = this,
      stream = new Stream,
      req,
      buff;

  stream.destroy = function () {
    req.destroy();
  };

  options = {
    method: 'stream',
    params: options
  };

  if (options.params.path) {
    options.path = options.params.path;
    delete options.params.path;
  }

  if (options.params.auth) {
    options.auth = options.params.auth;
    delete options.params.auth;
  }

  req = this._request(options);
  buff = '';

  req.on('data', function (data) {
    var data = (buff + data).split(/\n+/),
        l = data.length - 1,
        i = 0;

    for (; i < l; i++) {
      try {
        stream.emit('log', JSON.parse(data[i]));
      } catch (e) {
        stream.emit('error', e);
      }
    }

    buff = data[l];
  });

  req.on('error', function (err) {
    stream.emit('error', err);
  });

  return stream;
}
```
- example usage
```shell
...
## Streaming Logs
Streaming allows you to stream your logs back from your chosen transport.

''' js
  //
  // Start at the end.
  //
  winston.stream({ start: -1 }).on('log', function(log) {
    console.log(log);
  });
'''

## Exceptions

### Handling Uncaught Exceptions with winston
...
```



# <a name="apidoc.module.winston.transports.Memory"></a>[module winston.transports.Memory](#apidoc.module.winston.transports.Memory)

#### <a name="apidoc.element.winston.transports.Memory.Memory"></a>[function <span class="apidocSignatureSpan">winston.transports.</span>Memory (options)](#apidoc.element.winston.transports.Memory.Memory)
- description and source-code
```javascript
Memory = function (options) {
  Transport.call(this, options);
  options = options || {};

  this.errorOutput = [];
  this.writeOutput = [];

  this.json        = options.json        || false;
  this.colorize    = options.colorize    || false;
  this.prettyPrint = options.prettyPrint || false;
  this.timestamp   = typeof options.timestamp !== 'undefined' ? options.timestamp : false;
  this.showLevel   = options.showLevel === undefined ? true : options.showLevel;
  this.label       = options.label       || null;
  this.depth       = options.depth       || null;

  if (this.json) {
    this.stringify = options.stringify || function (obj) {
      return JSON.stringify(obj, null, 2);
    };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.Memory.super_"></a>[function <span class="apidocSignatureSpan">winston.transports.Memory.</span>super_ (options)](#apidoc.element.winston.transports.Memory.super_)
- description and source-code
```javascript
super_ = function (options) {
  events.EventEmitter.call(this);

  options        = options        || {};
  this.silent    = options.silent || false;
  this.raw       = options.raw    || false;
  this.name      = options.name   || this.name;
  this.formatter = options.formatter;

  //
  // Do not set a default level. When 'level' is falsey on any
  // 'Transport' instance, any 'Logger' instance uses the
  // configured level (instead of the Transport level)
  //
  this.level = options.level;

  this.handleExceptions = options.handleExceptions || false;
  this.exceptionsLevel  = options.exceptionsLevel || 'error';
  this.humanReadableUnhandledException = options.humanReadableUnhandledException || false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.winston.transports.Memory.prototype"></a>[module winston.transports.Memory.prototype](#apidoc.module.winston.transports.Memory.prototype)

#### <a name="apidoc.element.winston.transports.Memory.prototype.clearLogs"></a>[function <span class="apidocSignatureSpan">winston.transports.Memory.prototype.</span>clearLogs ()](#apidoc.element.winston.transports.Memory.prototype.clearLogs)
- description and source-code
```javascript
clearLogs = function () {
  this.errorOutput = [];
  this.writeOutput = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.winston.transports.Memory.prototype.log"></a>[function <span class="apidocSignatureSpan">winston.transports.Memory.prototype.</span>log (level, msg, meta, callback)](#apidoc.element.winston.transports.Memory.prototype.log)
- description and source-code
```javascript
log = function (level, msg, meta, callback) {
  if (this.silent) {
    return callback(null, true);
  }

  var self = this,
      output;

  output = common.log({
    colorize:    this.colorize,
    json:        this.json,
    level:       level,
    message:     msg,
    meta:        meta,
    stringify:   this.stringify,
    timestamp:   this.timestamp,
    prettyPrint: this.prettyPrint,
    raw:         this.raw,
    label:       this.label,
    depth:       this.depth,
    formatter:   this.formatter,
    humanReadableUnhandledException: this.humanReadableUnhandledException
  });

  if (level === 'error' || level === 'debug') {
    this.errorOutput.push(output);
  } else {
    this.writeOutput.push(output);
  }

  self.emit('logged');
  callback(null, true);
}
```
- example usage
```shell
...

### Using the Default Logger
The default logger is accessible through the winston module directly. Any method that you could call on an instance of a logger
is available on the default logger:

''' js
  var winston = require('winston');

  winston.log('info', 'Hello distributed log files!');
  winston.info('Hello again distributed logs');

  winston.level = 'debug';
  winston.log('debug', 'Now my debug messages are written to console!');
'''

By default, only the Console transport is set on the default logger. You can add or remove transports via the add() and remove()
methods:
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
