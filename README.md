# api documentation for  [ejs (v2.5.6)](https://github.com/mde/ejs)  [![npm package](https://img.shields.io/npm/v/npmdoc-ejs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ejs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ejs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ejs)
#### Embedded JavaScript templates

[![NPM](https://nodei.co/npm/ejs.png?downloads=true)](https://www.npmjs.com/package/ejs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ejs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-ejs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ejs/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ejs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ejs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matthew Eernisse",
        "email": "mde@fleegix.org",
        "url": "http://fleegix.org"
    },
    "bugs": {
        "url": "https://github.com/mde/ejs/issues"
    },
    "contributors": [
        {
            "name": "Timothy Gu",
            "email": "timothygu99@gmail.com",
            "url": "https://timothygu.github.io"
        }
    ],
    "dependencies": {},
    "description": "Embedded JavaScript templates",
    "devDependencies": {
        "browserify": "^13.0.1",
        "eslint": "^3.0.0",
        "git-directory-deploy": "^1.5.1",
        "istanbul": "~0.4.3",
        "jake": "^8.0.0",
        "jsdoc": "^3.4.0",
        "lru-cache": "^4.0.1",
        "mocha": "^3.0.2",
        "uglify-js": "^2.6.2"
    },
    "directories": {},
    "dist": {
        "shasum": "479636bfa3fe3b1debd52087f0acb204b4f19c88",
        "tarball": "https://registry.npmjs.org/ejs/-/ejs-2.5.6.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "homepage": "https://github.com/mde/ejs",
    "keywords": [
        "template",
        "engine",
        "ejs"
    ],
    "license": "Apache-2.0",
    "main": "./lib/ejs.js",
    "maintainers": [
        {
            "name": "mde",
            "email": "mde@fleegix.org"
        }
    ],
    "name": "ejs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mde/ejs.git"
    },
    "scripts": {
        "coverage": "istanbul cover node_modules/mocha/bin/_mocha",
        "devdoc": "jake doc[dev]",
        "doc": "jake doc",
        "lint": "eslint \"**/*.js\" Jakefile",
        "test": "mocha"
    },
    "version": "2.5.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ejs](#apidoc.module.ejs)
1.  [function <span class="apidocSignatureSpan">ejs.</span>__express ()](#apidoc.element.ejs.__express)
1.  [function <span class="apidocSignatureSpan">ejs.</span>clearCache ()](#apidoc.element.ejs.clearCache)
1.  [function <span class="apidocSignatureSpan">ejs.</span>compile (template, opts)](#apidoc.element.ejs.compile)
1.  [function <span class="apidocSignatureSpan">ejs.</span>escapeXML (markup)](#apidoc.element.ejs.escapeXML)
1.  [function <span class="apidocSignatureSpan">ejs.</span>fileLoader (path, options)](#apidoc.element.ejs.fileLoader)
1.  [function <span class="apidocSignatureSpan">ejs.</span>render (template, d, o)](#apidoc.element.ejs.render)
1.  [function <span class="apidocSignatureSpan">ejs.</span>renderFile ()](#apidoc.element.ejs.renderFile)
1.  [function <span class="apidocSignatureSpan">ejs.</span>resolveInclude (name, filename, isDir)](#apidoc.element.ejs.resolveInclude)
1.  object <span class="apidocSignatureSpan"></span>ejs
1.  object <span class="apidocSignatureSpan">ejs.</span>cache
1.  object <span class="apidocSignatureSpan">ejs.</span>utils
1.  string <span class="apidocSignatureSpan">ejs.</span>VERSION
1.  string <span class="apidocSignatureSpan">ejs.</span>localsName
1.  string <span class="apidocSignatureSpan">ejs.</span>name

#### [module ejs.cache](#apidoc.module.ejs.cache)
1.  [function <span class="apidocSignatureSpan">ejs.cache.</span>get (key)](#apidoc.element.ejs.cache.get)
1.  [function <span class="apidocSignatureSpan">ejs.cache.</span>reset ()](#apidoc.element.ejs.cache.reset)
1.  [function <span class="apidocSignatureSpan">ejs.cache.</span>set (key, val)](#apidoc.element.ejs.cache.set)
1.  object <span class="apidocSignatureSpan">ejs.cache.</span>_data

#### [module ejs.ejs](#apidoc.module.ejs.ejs)
1.  [function <span class="apidocSignatureSpan">ejs.ejs.</span>__express ()](#apidoc.element.ejs.ejs.__express)
1.  [function <span class="apidocSignatureSpan">ejs.ejs.</span>clearCache ()](#apidoc.element.ejs.ejs.clearCache)
1.  [function <span class="apidocSignatureSpan">ejs.ejs.</span>compile (template, opts)](#apidoc.element.ejs.ejs.compile)
1.  [function <span class="apidocSignatureSpan">ejs.ejs.</span>escapeXML (markup)](#apidoc.element.ejs.ejs.escapeXML)
1.  [function <span class="apidocSignatureSpan">ejs.ejs.</span>render (template, d, o)](#apidoc.element.ejs.ejs.render)
1.  [function <span class="apidocSignatureSpan">ejs.ejs.</span>renderFile ()](#apidoc.element.ejs.ejs.renderFile)
1.  [function <span class="apidocSignatureSpan">ejs.ejs.</span>resolveInclude (name, filename, isDir)](#apidoc.element.ejs.ejs.resolveInclude)
1.  object <span class="apidocSignatureSpan">ejs.ejs.</span>cache
1.  string <span class="apidocSignatureSpan">ejs.ejs.</span>VERSION
1.  string <span class="apidocSignatureSpan">ejs.ejs.</span>localsName
1.  string <span class="apidocSignatureSpan">ejs.ejs.</span>name

#### [module ejs.escapeXML](#apidoc.module.ejs.escapeXML)
1.  [function <span class="apidocSignatureSpan">ejs.</span>escapeXML (markup)](#apidoc.element.ejs.escapeXML.escapeXML)
1.  [function <span class="apidocSignatureSpan">ejs.escapeXML.</span>toString ()](#apidoc.element.ejs.escapeXML.toString)

#### [module ejs.utils](#apidoc.module.ejs.utils)
1.  [function <span class="apidocSignatureSpan">ejs.utils.</span>escapeRegExpChars (string)](#apidoc.element.ejs.utils.escapeRegExpChars)
1.  [function <span class="apidocSignatureSpan">ejs.utils.</span>escapeXML (markup)](#apidoc.element.ejs.utils.escapeXML)
1.  [function <span class="apidocSignatureSpan">ejs.utils.</span>shallowCopy (to, from)](#apidoc.element.ejs.utils.shallowCopy)
1.  [function <span class="apidocSignatureSpan">ejs.utils.</span>shallowCopyFromList (to, from, list)](#apidoc.element.ejs.utils.shallowCopyFromList)
1.  object <span class="apidocSignatureSpan">ejs.utils.</span>cache



# <a name="apidoc.module.ejs"></a>[module ejs](#apidoc.module.ejs)

#### <a name="apidoc.element.ejs.__express"></a>[function <span class="apidocSignatureSpan">ejs.</span>__express ()](#apidoc.element.ejs.__express)
- description and source-code
```javascript
__express = function () {
  var filename = arguments[0];
  var cb = arguments[arguments.length - 1];
  var opts = {filename: filename};
  var data;

  if (arguments.length > 2) {
    data = arguments[1];

    // No options object -- if there are optiony names
    // in the data, copy them to options
    if (arguments.length === 3) {
      // Express 4
      if (data.settings && data.settings['view options']) {
        utils.shallowCopyFromList(opts, data.settings['view options'], _OPTS_EXPRESS);
      }
      // Express 3 and lower
      else {
        utils.shallowCopyFromList(opts, data, _OPTS_EXPRESS);
      }
    }
    else {
      // Use shallowCopy so we don't pollute passed in opts obj with new vals
      utils.shallowCopy(opts, arguments[2]);
    }

    opts.filename = filename;
  }
  else {
    data = {};
  }

  return tryHandleCache(opts, data, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.clearCache"></a>[function <span class="apidocSignatureSpan">ejs.</span>clearCache ()](#apidoc.element.ejs.clearCache)
- description and source-code
```javascript
clearCache = function () {
  exports.cache.reset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.compile"></a>[function <span class="apidocSignatureSpan">ejs.</span>compile (template, opts)](#apidoc.element.ejs.compile)
- description and source-code
```javascript
function compile(template, opts) {
  var templ;

  // v1 compat
  // 'scope' is 'context'
  // FIXME: Remove this in a future version
  if (opts && opts.scope) {
    if (!scopeOptionWarned){
      console.warn(''scope' option is deprecated and will be removed in EJS 3');
      scopeOptionWarned = true;
    }
    if (!opts.context) {
      opts.context = opts.scope;
    }
    delete opts.scope;
  }
  templ = new Template(template, opts);
  return templ.compile();
}
```
- example usage
```shell
...
'''

Try EJS online at: https://ionicabizau.github.io/ejs-playground/.

## Usage

'''javascript
var template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
...
```

#### <a name="apidoc.element.ejs.escapeXML"></a>[function <span class="apidocSignatureSpan">ejs.</span>escapeXML (markup)](#apidoc.element.ejs.escapeXML)
- description and source-code
```javascript
escapeXML = function (markup) {
  return markup == undefined
    ? ''
    : String(markup)
        .replace(_MATCH_HTML, encode_char);
};
var _ENCODE_HTML_RULES = {
      "&": "&amp;"
    , "<": "&lt;"
    , ">": "&gt;"
    , '"': "&#34;"
    , "'": "&#39;"
    }
  , _MATCH_HTML = /[&<>'"]/g;
function encode_char(c) {
  return _ENCODE_HTML_RULES[c] || c;
};

```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.fileLoader"></a>[function <span class="apidocSignatureSpan">ejs.</span>fileLoader (path, options)](#apidoc.element.ejs.fileLoader)
- description and source-code
```javascript
fileLoader = function (path, options) {
  options = getOptions(options, { flag: 'r' });
  var isUserFd = isFd(path); // file descriptor ownership
  var fd = isUserFd ? path : fs.openSync(path, options.flag || 'r', 0o666);

  var st = tryStatSync(fd, isUserFd);
  var size = st.isFile() ? st.size : 0;
  var pos = 0;
  var buffer; // single buffer with file data
  var buffers; // list for when size is unknown

  if (size === 0) {
    buffers = [];
  } else {
    buffer = tryCreateBuffer(size, fd, isUserFd);
  }

  var bytesRead;

  if (size !== 0) {
    do {
      bytesRead = tryReadSync(fd, isUserFd, buffer, pos, size - pos);
      pos += bytesRead;
    } while (bytesRead !== 0 && pos < size);
  } else {
    do {
      // the kernel lies about many files.
      // Go ahead and try to read some bytes.
      buffer = Buffer.allocUnsafe(8192);
      bytesRead = tryReadSync(fd, isUserFd, buffer, 0, 8192);
      if (bytesRead !== 0) {
        buffers.push(buffer.slice(0, bytesRead));
      }
      pos += bytesRead;
    } while (bytesRead !== 0);
  }

  if (!isUserFd)
    fs.closeSync(fd);

  if (size === 0) {
    // data was collected into the buffers list.
    buffer = Buffer.concat(buffers, pos);
  } else if (pos < size) {
    buffer = buffer.slice(0, pos);
  }

  if (options.encoding) buffer = buffer.toString(options.encoding);
  return buffer;
}
```
- example usage
```shell
...
*
* @param {String} filePath ejs file path.
* @return {String} The contents of the specified file.
* @static
*/

function fileLoader(filePath){
 return exports.fileLoader(filePath);
}

/**
* Get the template function.
*
* If 'options.cache' is 'true', then the template is cached.
*
...
```

#### <a name="apidoc.element.ejs.render"></a>[function <span class="apidocSignatureSpan">ejs.</span>render (template, d, o)](#apidoc.element.ejs.render)
- description and source-code
```javascript
render = function (template, d, o) {
  var data = d || {};
  var opts = o || {};

  // No options object -- if there are optiony names
  // in the data, copy them to options
  if (arguments.length == 2) {
    utils.shallowCopyFromList(opts, data, _OPTS);
  }

  return handleCache(opts, template)(data);
}
```
- example usage
```shell
...
## Usage

'''javascript
var template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
});
'''
...
```

#### <a name="apidoc.element.ejs.renderFile"></a>[function <span class="apidocSignatureSpan">ejs.</span>renderFile ()](#apidoc.element.ejs.renderFile)
- description and source-code
```javascript
renderFile = function () {
  var filename = arguments[0];
  var cb = arguments[arguments.length - 1];
  var opts = {filename: filename};
  var data;

  if (arguments.length > 2) {
    data = arguments[1];

    // No options object -- if there are optiony names
    // in the data, copy them to options
    if (arguments.length === 3) {
      // Express 4
      if (data.settings && data.settings['view options']) {
        utils.shallowCopyFromList(opts, data.settings['view options'], _OPTS_EXPRESS);
      }
      // Express 3 and lower
      else {
        utils.shallowCopyFromList(opts, data, _OPTS_EXPRESS);
      }
    }
    else {
      // Use shallowCopy so we don't pollute passed in opts obj with new vals
      utils.shallowCopy(opts, arguments[2]);
    }

    opts.filename = filename;
  }
  else {
    data = {};
  }

  return tryHandleCache(opts, data, cb);
}
```
- example usage
```shell
...
var template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
});
'''

It is also possible to use 'ejs.render(dataAndOptions);' where you pass
everything in a single object. In that case, you'll end up with local variables
for all the passed options. However, be aware that your code could break if we
...
```

#### <a name="apidoc.element.ejs.resolveInclude"></a>[function <span class="apidocSignatureSpan">ejs.</span>resolveInclude (name, filename, isDir)](#apidoc.element.ejs.resolveInclude)
- description and source-code
```javascript
resolveInclude = function (name, filename, isDir) {
  var dirname = path.dirname;
  var extname = path.extname;
  var resolve = path.resolve;
  var includePath = resolve(isDir ? filename : dirname(filename), name);
  var ext = extname(name);
  if (!ext) {
    includePath += '.ejs';
  }
  return includePath;
}
```
- example usage
```shell
...
 * @param  {String}  path    specified path
 * @param  {Options} options compilation options
 * @return {String}
 */
function getIncludePath(path, options){
var includePath;
if (path.charAt(0) == '/') {
  includePath = exports.resolveInclude(path.replace(/^\/*/,''), options.root || '/', true);
}
else {
  if (!options.filename) {
    throw new Error(''include' use relative path requires the \'filename\' option.');
  }
  includePath = exports.resolveInclude(path, options.filename);
}
...
```



# <a name="apidoc.module.ejs.cache"></a>[module ejs.cache](#apidoc.module.ejs.cache)

#### <a name="apidoc.element.ejs.cache.get"></a>[function <span class="apidocSignatureSpan">ejs.cache.</span>get (key)](#apidoc.element.ejs.cache.get)
- description and source-code
```javascript
get = function (key) {
  return this._data[key];
}
```
- example usage
```shell
...
var filename = options.filename;
var hasTemplate = arguments.length > 1;

if (options.cache) {
  if (!filename) {
    throw new Error('cache option requires a filename');
  }
  func = exports.cache.get(filename);
  if (func) {
    return func;
  }
  if (!hasTemplate) {
    template = fileLoader(filename).toString().replace(_BOM, '');
  }
}
...
```

#### <a name="apidoc.element.ejs.cache.reset"></a>[function <span class="apidocSignatureSpan">ejs.cache.</span>reset ()](#apidoc.element.ejs.cache.reset)
- description and source-code
```javascript
reset = function () {
  this._data = {};
}
```
- example usage
```shell
...

/**
 * Clear intermediate JavaScript cache. Calls {@link Cache#reset}.
 * @public
 */

exports.clearCache = function () {
exports.cache.reset();
};

function Template(text, opts) {
opts = opts || {};
var options = {};
this.templateText = text;
this.mode = null;
...
```

#### <a name="apidoc.element.ejs.cache.set"></a>[function <span class="apidocSignatureSpan">ejs.cache.</span>set (key, val)](#apidoc.element.ejs.cache.set)
- description and source-code
```javascript
set = function (key, val) {
  this._data[key] = val;
}
```
- example usage
```shell
...
     throw new Error('Internal EJS error: no file name or template '
                   + 'provided');
   }
   template = fileLoader(filename).toString().replace(_BOM, '');
 }
 func = exports.compile(template, options);
 if (options.cache) {
   exports.cache.set(filename, func);
 }
 return func;
}

/**
* Try calling handleCache with the given options and data and call the
* callback with the result. If an error occurs, call the callback with
...
```



# <a name="apidoc.module.ejs.ejs"></a>[module ejs.ejs](#apidoc.module.ejs.ejs)

#### <a name="apidoc.element.ejs.ejs.__express"></a>[function <span class="apidocSignatureSpan">ejs.ejs.</span>__express ()](#apidoc.element.ejs.ejs.__express)
- description and source-code
```javascript
__express = function () {
  var filename = arguments[0];
  var cb = arguments[arguments.length - 1];
  var opts = {filename: filename};
  var data;

  if (arguments.length > 2) {
    data = arguments[1];

    // No options object -- if there are optiony names
    // in the data, copy them to options
    if (arguments.length === 3) {
      // Express 4
      if (data.settings && data.settings['view options']) {
        utils.shallowCopyFromList(opts, data.settings['view options'], _OPTS_EXPRESS);
      }
      // Express 3 and lower
      else {
        utils.shallowCopyFromList(opts, data, _OPTS_EXPRESS);
      }
    }
    else {
      // Use shallowCopy so we don't pollute passed in opts obj with new vals
      utils.shallowCopy(opts, arguments[2]);
    }

    opts.filename = filename;
  }
  else {
    data = {};
  }

  return tryHandleCache(opts, data, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.ejs.clearCache"></a>[function <span class="apidocSignatureSpan">ejs.ejs.</span>clearCache ()](#apidoc.element.ejs.ejs.clearCache)
- description and source-code
```javascript
clearCache = function () {
  exports.cache.reset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.ejs.compile"></a>[function <span class="apidocSignatureSpan">ejs.ejs.</span>compile (template, opts)](#apidoc.element.ejs.ejs.compile)
- description and source-code
```javascript
function compile(template, opts) {
  var templ;

  // v1 compat
  // 'scope' is 'context'
  // FIXME: Remove this in a future version
  if (opts && opts.scope) {
    if (!scopeOptionWarned){
      console.warn(''scope' option is deprecated and will be removed in EJS 3');
      scopeOptionWarned = true;
    }
    if (!opts.context) {
      opts.context = opts.scope;
    }
    delete opts.scope;
  }
  templ = new Template(template, opts);
  return templ.compile();
}
```
- example usage
```shell
...
'''

Try EJS online at: https://ionicabizau.github.io/ejs-playground/.

## Usage

'''javascript
var template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
...
```

#### <a name="apidoc.element.ejs.ejs.escapeXML"></a>[function <span class="apidocSignatureSpan">ejs.ejs.</span>escapeXML (markup)](#apidoc.element.ejs.ejs.escapeXML)
- description and source-code
```javascript
escapeXML = function (markup) {
  return markup == undefined
    ? ''
    : String(markup)
        .replace(_MATCH_HTML, encode_char);
};
var _ENCODE_HTML_RULES = {
      "&": "&amp;"
    , "<": "&lt;"
    , ">": "&gt;"
    , '"': "&#34;"
    , "'": "&#39;"
    }
  , _MATCH_HTML = /[&<>'"]/g;
function encode_char(c) {
  return _ENCODE_HTML_RULES[c] || c;
};

```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.ejs.render"></a>[function <span class="apidocSignatureSpan">ejs.ejs.</span>render (template, d, o)](#apidoc.element.ejs.ejs.render)
- description and source-code
```javascript
render = function (template, d, o) {
  var data = d || {};
  var opts = o || {};

  // No options object -- if there are optiony names
  // in the data, copy them to options
  if (arguments.length == 2) {
    utils.shallowCopyFromList(opts, data, _OPTS);
  }

  return handleCache(opts, template)(data);
}
```
- example usage
```shell
...
## Usage

'''javascript
var template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
});
'''
...
```

#### <a name="apidoc.element.ejs.ejs.renderFile"></a>[function <span class="apidocSignatureSpan">ejs.ejs.</span>renderFile ()](#apidoc.element.ejs.ejs.renderFile)
- description and source-code
```javascript
renderFile = function () {
  var filename = arguments[0];
  var cb = arguments[arguments.length - 1];
  var opts = {filename: filename};
  var data;

  if (arguments.length > 2) {
    data = arguments[1];

    // No options object -- if there are optiony names
    // in the data, copy them to options
    if (arguments.length === 3) {
      // Express 4
      if (data.settings && data.settings['view options']) {
        utils.shallowCopyFromList(opts, data.settings['view options'], _OPTS_EXPRESS);
      }
      // Express 3 and lower
      else {
        utils.shallowCopyFromList(opts, data, _OPTS_EXPRESS);
      }
    }
    else {
      // Use shallowCopy so we don't pollute passed in opts obj with new vals
      utils.shallowCopy(opts, arguments[2]);
    }

    opts.filename = filename;
  }
  else {
    data = {};
  }

  return tryHandleCache(opts, data, cb);
}
```
- example usage
```shell
...
var template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
});
'''

It is also possible to use 'ejs.render(dataAndOptions);' where you pass
everything in a single object. In that case, you'll end up with local variables
for all the passed options. However, be aware that your code could break if we
...
```

#### <a name="apidoc.element.ejs.ejs.resolveInclude"></a>[function <span class="apidocSignatureSpan">ejs.ejs.</span>resolveInclude (name, filename, isDir)](#apidoc.element.ejs.ejs.resolveInclude)
- description and source-code
```javascript
resolveInclude = function (name, filename, isDir) {
  var dirname = path.dirname;
  var extname = path.extname;
  var resolve = path.resolve;
  var includePath = resolve(isDir ? filename : dirname(filename), name);
  var ext = extname(name);
  if (!ext) {
    includePath += '.ejs';
  }
  return includePath;
}
```
- example usage
```shell
...
 * @param  {String}  path    specified path
 * @param  {Options} options compilation options
 * @return {String}
 */
function getIncludePath(path, options){
var includePath;
if (path.charAt(0) == '/') {
  includePath = exports.resolveInclude(path.replace(/^\/*/,''), options.root || '/', true);
}
else {
  if (!options.filename) {
    throw new Error(''include' use relative path requires the \'filename\' option.');
  }
  includePath = exports.resolveInclude(path, options.filename);
}
...
```



# <a name="apidoc.module.ejs.escapeXML"></a>[module ejs.escapeXML](#apidoc.module.ejs.escapeXML)

#### <a name="apidoc.element.ejs.escapeXML.escapeXML"></a>[function <span class="apidocSignatureSpan">ejs.</span>escapeXML (markup)](#apidoc.element.ejs.escapeXML.escapeXML)
- description and source-code
```javascript
escapeXML = function (markup) {
  return markup == undefined
    ? ''
    : String(markup)
        .replace(_MATCH_HTML, encode_char);
};
var _ENCODE_HTML_RULES = {
      "&": "&amp;"
    , "<": "&lt;"
    , ">": "&gt;"
    , '"': "&#34;"
    , "'": "&#39;"
    }
  , _MATCH_HTML = /[&<>'"]/g;
function encode_char(c) {
  return _ENCODE_HTML_RULES[c] || c;
};

```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.escapeXML.toString"></a>[function <span class="apidocSignatureSpan">ejs.escapeXML.</span>toString ()](#apidoc.element.ejs.escapeXML.toString)
- description and source-code
```javascript
toString = function () {
  return Function.prototype.toString.call(this) + ';\n' + escapeFuncStr;
}
```
- example usage
```shell
...
  - '_with'           Whether or not to use 'with() {}' constructs. If 'false' then the locals will be stored in the 'locals' object
. Set to 'false' in strict mode.
  - 'localsName'      Name to use for the object storing local variables when not using 'with' Defaults to 'locals'
  - 'rmWhitespace'    Remove all safe-to-remove whitespace, including leading
    and trailing whitespace. It also enables a safer version of '-%>' line
    slurping for all scriptlet tags (it does not strip new lines of tags in
    the middle of a line).
  - 'escape'          The escaping function used with '<%=' construct. It is
    used in rendering and is '.toString()'ed in the generation of client functions. (By default escapes XML).

This project uses [JSDoc](http://usejsdoc.org/). For the full public API
documentation, clone the repository and run 'npm run doc'. This will run JSDoc
with the proper options and output the documentation to 'out/'. If you want
the both the public & private API docs, run 'npm run devdoc' instead.

## Tags
...
```



# <a name="apidoc.module.ejs.utils"></a>[module ejs.utils](#apidoc.module.ejs.utils)

#### <a name="apidoc.element.ejs.utils.escapeRegExpChars"></a>[function <span class="apidocSignatureSpan">ejs.utils.</span>escapeRegExpChars (string)](#apidoc.element.ejs.utils.escapeRegExpChars)
- description and source-code
```javascript
escapeRegExpChars = function (string) {
  // istanbul ignore if
  if (!string) {
    return '';
  }
  return String(string).replace(regExpChars, '\\$&');
}
```
- example usage
```shell
...
COMMENT: 'comment',
LITERAL: 'literal'
};

Template.prototype = {
createRegex: function () {
  var str = _REGEX_STRING;
  var delim = utils.escapeRegExpChars(this.opts.delimiter);
  str = str.replace(/%/g, delim);
  return new RegExp(str);
},

compile: function () {
  var src;
  var fn;
...
```

#### <a name="apidoc.element.ejs.utils.escapeXML"></a>[function <span class="apidocSignatureSpan">ejs.utils.</span>escapeXML (markup)](#apidoc.element.ejs.utils.escapeXML)
- description and source-code
```javascript
escapeXML = function (markup) {
  return markup == undefined
    ? ''
    : String(markup)
        .replace(_MATCH_HTML, encode_char);
};
var _ENCODE_HTML_RULES = {
      "&": "&amp;"
    , "<": "&lt;"
    , ">": "&gt;"
    , '"': "&#34;"
    , "'": "&#39;"
    }
  , _MATCH_HTML = /[&<>'"]/g;
function encode_char(c) {
  return _ENCODE_HTML_RULES[c] || c;
};

```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ejs.utils.shallowCopy"></a>[function <span class="apidocSignatureSpan">ejs.utils.</span>shallowCopy (to, from)](#apidoc.element.ejs.utils.shallowCopy)
- description and source-code
```javascript
shallowCopy = function (to, from) {
  from = from || {};
  for (var p in from) {
    to[p] = from[p];
  }
  return to;
}
```
- example usage
```shell
...
* @param {Options} options compilation options
* @return {(TemplateFunction|ClientFunction)}
* Depending on the value of 'options.client', either type might be returned
* @static
*/

function includeFile(path, options) {
 var opts = utils.shallowCopy({}, options);
 opts.filename = getIncludePath(path, opts);
 return handleCache(opts);
}

/**
* Get the JavaScript source of an included file.
*
...
```

#### <a name="apidoc.element.ejs.utils.shallowCopyFromList"></a>[function <span class="apidocSignatureSpan">ejs.utils.</span>shallowCopyFromList (to, from, list)](#apidoc.element.ejs.utils.shallowCopyFromList)
- description and source-code
```javascript
shallowCopyFromList = function (to, from, list) {
  for (var i = 0; i < list.length; i++) {
    var p = list[i];
    if (typeof from[p] != 'undefined') {
      to[p] = from[p];
    }
  }
  return to;
}
```
- example usage
```shell
...
exports.render = function (template, d, o) {
 var data = d || {};
 var opts = o || {};

 // No options object -- if there are optiony names
 // in the data, copy them to options
 if (arguments.length == 2) {
   utils.shallowCopyFromList(opts, data, _OPTS);
 }

 return handleCache(opts, template)(data);
};

/**
* Render an EJS file at the given 'path' and callback 'cb(err, str)'.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
