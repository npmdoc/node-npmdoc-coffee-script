# api documentation for  [coffee-script (v1.12.4)](http://coffeescript.org)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-coffee-script.svg)](https://travis-ci.org/npmdoc/node-npmdoc-coffee-script)
#### Unfancy JavaScript

[![NPM](https://nodei.co/npm/coffee-script.png?downloads=true)](https://www.npmjs.com/package/coffee-script)

[![apidoc](https://npmdoc.github.io/node-npmdoc-coffee-script/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-coffee-script_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-coffee-script/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-coffee-script/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Jeremy Ashkenas"
    },
    "bin": {
        "coffee": "./bin/coffee",
        "cake": "./bin/cake"
    },
    "bugs": {
        "url": "https://github.com/jashkenas/coffeescript/issues"
    },
    "dependencies": {},
    "description": "Unfancy JavaScript",
    "devDependencies": {
        "docco": "~0.7.0",
        "google-closure-compiler-js": "^20170124.0.0",
        "highlight.js": "~9.9.0",
        "jison": ">=0.4.17",
        "marked": "^0.3.6",
        "underscore": "~1.8.3"
    },
    "directories": {
        "lib": "./lib/coffee-script"
    },
    "dist": {
        "shasum": "fe1bced97fe1fb3927b998f2b45616e0658be1ff",
        "tarball": "https://registry.npmjs.org/coffee-script/-/coffee-script-1.12.4.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "files": [
        "bin",
        "lib",
        "register.js",
        "repl.js"
    ],
    "gitHead": "91e3f7255c3bc6e7100329a98271227719f0153c",
    "homepage": "http://coffeescript.org",
    "keywords": [
        "javascript",
        "language",
        "coffeescript",
        "compiler"
    ],
    "license": "MIT",
    "main": "./lib/coffee-script/coffee-script",
    "maintainers": [
        {
            "name": "jashkenas",
            "email": "jashkenas@gmail.com"
        },
        {
            "name": "lydell",
            "email": "simon.lydell@gmail.com"
        },
        {
            "name": "michaelficarra",
            "email": "npm@michael.ficarra.me"
        }
    ],
    "name": "coffee-script",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jashkenas/coffeescript.git"
    },
    "scripts": {
        "test": "node ./bin/cake test",
        "test-harmony": "node --harmony ./bin/cake test"
    },
    "version": "1.12.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module coffee-script](#apidoc.module.coffee-script)
1.  [function <span class="apidocSignatureSpan">coffee-script.</span>_compileFile (filename, sourceMap, inlineMap)](#apidoc.element.coffee-script._compileFile)
1.  [function <span class="apidocSignatureSpan">coffee-script.</span>compile (code, options)](#apidoc.element.coffee-script.compile)
1.  [function <span class="apidocSignatureSpan">coffee-script.</span>eval (code, options)](#apidoc.element.coffee-script.eval)
1.  [function <span class="apidocSignatureSpan">coffee-script.</span>nodes (code, options)](#apidoc.element.coffee-script.nodes)
1.  [function <span class="apidocSignatureSpan">coffee-script.</span>register ()](#apidoc.element.coffee-script.register)
1.  [function <span class="apidocSignatureSpan">coffee-script.</span>run (code, options)](#apidoc.element.coffee-script.run)
1.  [function <span class="apidocSignatureSpan">coffee-script.</span>tokens (code, options)](#apidoc.element.coffee-script.tokens)
1.  object <span class="apidocSignatureSpan">coffee-script.</span>FILE_EXTENSIONS
1.  object <span class="apidocSignatureSpan">coffee-script.</span>coffee_script
1.  object <span class="apidocSignatureSpan">coffee-script.</span>helpers
1.  string <span class="apidocSignatureSpan">coffee-script.</span>VERSION

#### [module coffee-script.coffee_script](#apidoc.module.coffee-script.coffee_script)
1.  [function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>_compileFile (filename, sourceMap, inlineMap)](#apidoc.element.coffee-script.coffee_script._compileFile)
1.  [function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>compile (code, options)](#apidoc.element.coffee-script.coffee_script.compile)
1.  [function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>eval (code, options)](#apidoc.element.coffee-script.coffee_script.eval)
1.  [function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>nodes (code, options)](#apidoc.element.coffee-script.coffee_script.nodes)
1.  [function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>register ()](#apidoc.element.coffee-script.coffee_script.register)
1.  [function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>run (code, options)](#apidoc.element.coffee-script.coffee_script.run)
1.  [function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>tokens (code, options)](#apidoc.element.coffee-script.coffee_script.tokens)
1.  object <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>FILE_EXTENSIONS
1.  object <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>helpers
1.  string <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>VERSION

#### [module coffee-script.helpers](#apidoc.module.coffee-script.helpers)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>addLocationDataFn (first, last)](#apidoc.element.coffee-script.helpers.addLocationDataFn)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>baseFileName (file, stripExt, useWinPathSep)](#apidoc.element.coffee-script.helpers.baseFileName)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>compact (array)](#apidoc.element.coffee-script.helpers.compact)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>count (string, substr)](#apidoc.element.coffee-script.helpers.count)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>del (obj, key)](#apidoc.element.coffee-script.helpers.del)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>ends (string, literal, back)](#apidoc.element.coffee-script.helpers.ends)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>extend (object, properties)](#apidoc.element.coffee-script.helpers.extend)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>flatten (array)](#apidoc.element.coffee-script.helpers.flatten)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>invertLiterate (code)](#apidoc.element.coffee-script.helpers.invertLiterate)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>isCoffee (file)](#apidoc.element.coffee-script.helpers.isCoffee)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>isLiterate (file)](#apidoc.element.coffee-script.helpers.isLiterate)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>locationDataToString (obj)](#apidoc.element.coffee-script.helpers.locationDataToString)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>merge (options, overrides)](#apidoc.element.coffee-script.helpers.merge)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>nameWhitespaceCharacter (string)](#apidoc.element.coffee-script.helpers.nameWhitespaceCharacter)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>repeat (str, n)](#apidoc.element.coffee-script.helpers.repeat)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>some ()](#apidoc.element.coffee-script.helpers.some)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>starts (string, literal, start)](#apidoc.element.coffee-script.helpers.starts)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>throwSyntaxError (message, location)](#apidoc.element.coffee-script.helpers.throwSyntaxError)
1.  [function <span class="apidocSignatureSpan">coffee-script.helpers.</span>updateSyntaxError (error, code, filename)](#apidoc.element.coffee-script.helpers.updateSyntaxError)



# <a name="apidoc.module.coffee-script"></a>[module coffee-script](#apidoc.module.coffee-script)

#### <a name="apidoc.element.coffee-script._compileFile"></a>[function <span class="apidocSignatureSpan">coffee-script.</span>_compileFile (filename, sourceMap, inlineMap)](#apidoc.element.coffee-script._compileFile)
- description and source-code
```javascript
_compileFile = function (filename, sourceMap, inlineMap) {
  var answer, err, raw, stripped;
  if (sourceMap == null) {
    sourceMap = false;
  }
  if (inlineMap == null) {
    inlineMap = false;
  }
  raw = fs.readFileSync(filename, 'utf8');
  stripped = raw.charCodeAt(0) === 0xFEFF ? raw.substring(1) : raw;
  try {
    answer = compile(stripped, {
      filename: filename,
      sourceMap: sourceMap,
      inlineMap: inlineMap,
      sourceFiles: [filename],
      literate: helpers.isLiterate(filename)
    });
  } catch (error) {
    err = error;
    throw helpers.updateSyntaxError(err, stripped, filename);
  }
  return answer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.compile"></a>[function <span class="apidocSignatureSpan">coffee-script.</span>compile (code, options)](#apidoc.element.coffee-script.compile)
- description and source-code
```javascript
compile = function (code, options) {
  var err;
  if (options == null) {
    options = {};
  }
  try {
    return fn.call(this, code, options);
  } catch (error) {
    err = error;
    if (typeof code !== 'string') {
      throw err;
    }
    throw helpers.updateSyntaxError(err, code, options.filename);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.eval"></a>[function <span class="apidocSignatureSpan">coffee-script.</span>eval (code, options)](#apidoc.element.coffee-script.eval)
- description and source-code
```javascript
eval = function (code, options) {
  var Module, _module, _require, createContext, i, isContext, js, k, len, o, r, ref, ref1, ref2, ref3, sandbox, v;
  if (options == null) {
    options = {};
  }
  if (!(code = code.trim())) {
    return;
  }
  createContext = (ref = vm.Script.createContext) != null ? ref : vm.createContext;
  isContext = (ref1 = vm.isContext) != null ? ref1 : function(ctx) {
    return options.sandbox instanceof createContext().constructor;
  };
  if (createContext) {
    if (options.sandbox != null) {
      if (isContext(options.sandbox)) {
        sandbox = options.sandbox;
      } else {
        sandbox = createContext();
        ref2 = options.sandbox;
        for (k in ref2) {
          if (!hasProp.call(ref2, k)) continue;
          v = ref2[k];
          sandbox[k] = v;
        }
      }
      sandbox.global = sandbox.root = sandbox.GLOBAL = sandbox;
    } else {
      sandbox = global;
    }
    sandbox.__filename = options.filename || 'eval';
    sandbox.__dirname = path.dirname(sandbox.__filename);
    if (!(sandbox !== global || sandbox.module || sandbox.require)) {
      Module = require('module');
      sandbox.module = _module = new Module(options.modulename || 'eval');
      sandbox.require = _require = function(path) {
        return Module._load(path, _module, true);
      };
      _module.filename = sandbox.__filename;
      ref3 = Object.getOwnPropertyNames(require);
      for (i = 0, len = ref3.length; i < len; i++) {
        r = ref3[i];
        if (r !== 'paths' && r !== 'arguments' && r !== 'caller') {
          _require[r] = require[r];
        }
      }
      _require.paths = _module.paths = Module._nodeModulePaths(process.cwd());
      _require.resolve = function(request) {
        return Module._resolveFilename(request, _module);
      };
    }
  }
  o = {};
  for (k in options) {
    if (!hasProp.call(options, k)) continue;
    v = options[k];
    o[k] = v;
  }
  o.bare = true;
  js = compile(code, o);
  if (sandbox === global) {
    return vm.runInThisContext(js);
  } else {
    return vm.runInContext(js, sandbox);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.nodes"></a>[function <span class="apidocSignatureSpan">coffee-script.</span>nodes (code, options)](#apidoc.element.coffee-script.nodes)
- description and source-code
```javascript
nodes = function (code, options) {
  var err;
  if (options == null) {
    options = {};
  }
  try {
    return fn.call(this, code, options);
  } catch (error) {
    err = error;
    if (typeof code !== 'string') {
      throw err;
    }
    throw helpers.updateSyntaxError(err, code, options.filename);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.register"></a>[function <span class="apidocSignatureSpan">coffee-script.</span>register ()](#apidoc.element.coffee-script.register)
- description and source-code
```javascript
register = function () {
  return require('./register');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.run"></a>[function <span class="apidocSignatureSpan">coffee-script.</span>run (code, options)](#apidoc.element.coffee-script.run)
- description and source-code
```javascript
run = function (code, options) {
  var answer, dir, mainModule, ref;
  if (options == null) {
    options = {};
  }
  mainModule = require.main;
  mainModule.filename = process.argv[1] = options.filename ? fs.realpathSync(options.filename) : '<anonymous>';
  mainModule.moduleCache && (mainModule.moduleCache = {});
  dir = options.filename != null ? path.dirname(fs.realpathSync(options.filename)) : fs.realpathSync('.');
  mainModule.paths = require('module')._nodeModulePaths(dir);
  if (!helpers.isCoffee(mainModule.filename) || require.extensions) {
    answer = compile(code, options);
    code = (ref = answer.js) != null ? ref : answer;
  }
  return mainModule._compile(code, mainModule.filename);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.tokens"></a>[function <span class="apidocSignatureSpan">coffee-script.</span>tokens (code, options)](#apidoc.element.coffee-script.tokens)
- description and source-code
```javascript
tokens = function (code, options) {
  var err;
  if (options == null) {
    options = {};
  }
  try {
    return fn.call(this, code, options);
  } catch (error) {
    err = error;
    if (typeof code !== 'string') {
      throw err;
    }
    throw helpers.updateSyntaxError(err, code, options.filename);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.coffee-script.coffee_script"></a>[module coffee-script.coffee_script](#apidoc.module.coffee-script.coffee_script)

#### <a name="apidoc.element.coffee-script.coffee_script._compileFile"></a>[function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>_compileFile (filename, sourceMap, inlineMap)](#apidoc.element.coffee-script.coffee_script._compileFile)
- description and source-code
```javascript
_compileFile = function (filename, sourceMap, inlineMap) {
  var answer, err, raw, stripped;
  if (sourceMap == null) {
    sourceMap = false;
  }
  if (inlineMap == null) {
    inlineMap = false;
  }
  raw = fs.readFileSync(filename, 'utf8');
  stripped = raw.charCodeAt(0) === 0xFEFF ? raw.substring(1) : raw;
  try {
    answer = compile(stripped, {
      filename: filename,
      sourceMap: sourceMap,
      inlineMap: inlineMap,
      sourceFiles: [filename],
      literate: helpers.isLiterate(filename)
    });
  } catch (error) {
    err = error;
    throw helpers.updateSyntaxError(err, stripped, filename);
  }
  return answer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.coffee_script.compile"></a>[function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>compile (code, options)](#apidoc.element.coffee-script.coffee_script.compile)
- description and source-code
```javascript
compile = function (code, options) {
  var err;
  if (options == null) {
    options = {};
  }
  try {
    return fn.call(this, code, options);
  } catch (error) {
    err = error;
    if (typeof code !== 'string') {
      throw err;
    }
    throw helpers.updateSyntaxError(err, code, options.filename);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.coffee_script.eval"></a>[function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>eval (code, options)](#apidoc.element.coffee-script.coffee_script.eval)
- description and source-code
```javascript
eval = function (code, options) {
  var Module, _module, _require, createContext, i, isContext, js, k, len, o, r, ref, ref1, ref2, ref3, sandbox, v;
  if (options == null) {
    options = {};
  }
  if (!(code = code.trim())) {
    return;
  }
  createContext = (ref = vm.Script.createContext) != null ? ref : vm.createContext;
  isContext = (ref1 = vm.isContext) != null ? ref1 : function(ctx) {
    return options.sandbox instanceof createContext().constructor;
  };
  if (createContext) {
    if (options.sandbox != null) {
      if (isContext(options.sandbox)) {
        sandbox = options.sandbox;
      } else {
        sandbox = createContext();
        ref2 = options.sandbox;
        for (k in ref2) {
          if (!hasProp.call(ref2, k)) continue;
          v = ref2[k];
          sandbox[k] = v;
        }
      }
      sandbox.global = sandbox.root = sandbox.GLOBAL = sandbox;
    } else {
      sandbox = global;
    }
    sandbox.__filename = options.filename || 'eval';
    sandbox.__dirname = path.dirname(sandbox.__filename);
    if (!(sandbox !== global || sandbox.module || sandbox.require)) {
      Module = require('module');
      sandbox.module = _module = new Module(options.modulename || 'eval');
      sandbox.require = _require = function(path) {
        return Module._load(path, _module, true);
      };
      _module.filename = sandbox.__filename;
      ref3 = Object.getOwnPropertyNames(require);
      for (i = 0, len = ref3.length; i < len; i++) {
        r = ref3[i];
        if (r !== 'paths' && r !== 'arguments' && r !== 'caller') {
          _require[r] = require[r];
        }
      }
      _require.paths = _module.paths = Module._nodeModulePaths(process.cwd());
      _require.resolve = function(request) {
        return Module._resolveFilename(request, _module);
      };
    }
  }
  o = {};
  for (k in options) {
    if (!hasProp.call(options, k)) continue;
    v = options[k];
    o[k] = v;
  }
  o.bare = true;
  js = compile(code, o);
  if (sandbox === global) {
    return vm.runInThisContext(js);
  } else {
    return vm.runInContext(js, sandbox);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.coffee_script.nodes"></a>[function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>nodes (code, options)](#apidoc.element.coffee-script.coffee_script.nodes)
- description and source-code
```javascript
nodes = function (code, options) {
  var err;
  if (options == null) {
    options = {};
  }
  try {
    return fn.call(this, code, options);
  } catch (error) {
    err = error;
    if (typeof code !== 'string') {
      throw err;
    }
    throw helpers.updateSyntaxError(err, code, options.filename);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.coffee_script.register"></a>[function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>register ()](#apidoc.element.coffee-script.coffee_script.register)
- description and source-code
```javascript
register = function () {
  return require('./register');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.coffee_script.run"></a>[function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>run (code, options)](#apidoc.element.coffee-script.coffee_script.run)
- description and source-code
```javascript
run = function (code, options) {
  var answer, dir, mainModule, ref;
  if (options == null) {
    options = {};
  }
  mainModule = require.main;
  mainModule.filename = process.argv[1] = options.filename ? fs.realpathSync(options.filename) : '<anonymous>';
  mainModule.moduleCache && (mainModule.moduleCache = {});
  dir = options.filename != null ? path.dirname(fs.realpathSync(options.filename)) : fs.realpathSync('.');
  mainModule.paths = require('module')._nodeModulePaths(dir);
  if (!helpers.isCoffee(mainModule.filename) || require.extensions) {
    answer = compile(code, options);
    code = (ref = answer.js) != null ? ref : answer;
  }
  return mainModule._compile(code, mainModule.filename);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.coffee_script.tokens"></a>[function <span class="apidocSignatureSpan">coffee-script.coffee_script.</span>tokens (code, options)](#apidoc.element.coffee-script.coffee_script.tokens)
- description and source-code
```javascript
tokens = function (code, options) {
  var err;
  if (options == null) {
    options = {};
  }
  try {
    return fn.call(this, code, options);
  } catch (error) {
    err = error;
    if (typeof code !== 'string') {
      throw err;
    }
    throw helpers.updateSyntaxError(err, code, options.filename);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.coffee-script.helpers"></a>[module coffee-script.helpers](#apidoc.module.coffee-script.helpers)

#### <a name="apidoc.element.coffee-script.helpers.addLocationDataFn"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>addLocationDataFn (first, last)](#apidoc.element.coffee-script.helpers.addLocationDataFn)
- description and source-code
```javascript
addLocationDataFn = function (first, last) {
  return function(obj) {
    if (((typeof obj) === 'object') && (!!obj['updateLocationDataIfMissing'])) {
      obj.updateLocationDataIfMissing(buildLocationData(first, last));
    }
    return obj;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.baseFileName"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>baseFileName (file, stripExt, useWinPathSep)](#apidoc.element.coffee-script.helpers.baseFileName)
- description and source-code
```javascript
baseFileName = function (file, stripExt, useWinPathSep) {
  var parts, pathSep;
  if (stripExt == null) {
    stripExt = false;
  }
  if (useWinPathSep == null) {
    useWinPathSep = false;
  }
  pathSep = useWinPathSep ? /\\|\// : /\//;
  parts = file.split(pathSep);
  file = parts[parts.length - 1];
  if (!(stripExt && file.indexOf('.') >= 0)) {
    return file;
  }
  parts = file.split('.');
  parts.pop();
  if (parts[parts.length - 1] === 'coffee' && parts.length > 1) {
    parts.pop();
  }
  return parts.join('.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.compact"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>compact (array)](#apidoc.element.coffee-script.helpers.compact)
- description and source-code
```javascript
compact = function (array) {
  var i, item, len1, results;
  results = [];
  for (i = 0, len1 = array.length; i < len1; i++) {
    item = array[i];
    if (item) {
      results.push(item);
    }
  }
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.count"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>count (string, substr)](#apidoc.element.coffee-script.helpers.count)
- description and source-code
```javascript
count = function (string, substr) {
  var num, pos;
  num = pos = 0;
  if (!substr.length) {
    return 1 / 0;
  }
  while (pos = 1 + string.indexOf(substr, pos)) {
    num++;
  }
  return num;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.del"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>del (obj, key)](#apidoc.element.coffee-script.helpers.del)
- description and source-code
```javascript
del = function (obj, key) {
  var val;
  val = obj[key];
  delete obj[key];
  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.ends"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>ends (string, literal, back)](#apidoc.element.coffee-script.helpers.ends)
- description and source-code
```javascript
ends = function (string, literal, back) {
  var len;
  len = literal.length;
  return literal === string.substr(string.length - len - (back || 0), len);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.extend"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>extend (object, properties)](#apidoc.element.coffee-script.helpers.extend)
- description and source-code
```javascript
extend = function (object, properties) {
  var key, val;
  for (key in properties) {
    val = properties[key];
    object[key] = val;
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.flatten"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>flatten (array)](#apidoc.element.coffee-script.helpers.flatten)
- description and source-code
```javascript
flatten = function (array) {
  var element, flattened, i, len1;
  flattened = [];
  for (i = 0, len1 = array.length; i < len1; i++) {
    element = array[i];
    if ('[object Array]' === Object.prototype.toString.call(element)) {
      flattened = flattened.concat(flatten(element));
    } else {
      flattened.push(element);
    }
  }
  return flattened;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.invertLiterate"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>invertLiterate (code)](#apidoc.element.coffee-script.helpers.invertLiterate)
- description and source-code
```javascript
invertLiterate = function (code) {
  var line, lines, maybe_code;
  maybe_code = true;
  lines = (function() {
    var i, len1, ref1, results;
    ref1 = code.split('\n');
    results = [];
    for (i = 0, len1 = ref1.length; i < len1; i++) {
      line = ref1[i];
      if (maybe_code && /^([ ]{4}|[ ]{0,3}\t)/.test(line)) {
        results.push(line);
      } else if (maybe_code = /^\s*$/.test(line)) {
        results.push(line);
      } else {
        results.push('# ' + line);
      }
    }
    return results;
  })();
  return lines.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.isCoffee"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>isCoffee (file)](#apidoc.element.coffee-script.helpers.isCoffee)
- description and source-code
```javascript
isCoffee = function (file) {
  return /\.((lit)?coffee|coffee\.md)$/.test(file);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.isLiterate"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>isLiterate (file)](#apidoc.element.coffee-script.helpers.isLiterate)
- description and source-code
```javascript
isLiterate = function (file) {
  return /\.(litcoffee|coffee\.md)$/.test(file);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.locationDataToString"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>locationDataToString (obj)](#apidoc.element.coffee-script.helpers.locationDataToString)
- description and source-code
```javascript
locationDataToString = function (obj) {
  var locationData;
  if (("2" in obj) && ("first_line" in obj[2])) {
    locationData = obj[2];
  } else if ("first_line" in obj) {
    locationData = obj;
  }
  if (locationData) {
    return ((locationData.first_line + 1) + ":" + (locationData.first_column + 1) + "-") + ((locationData.last_line + 1) + ":" + (
locationData.last_column + 1));
  } else {
    return "No location data";
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.merge"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>merge (options, overrides)](#apidoc.element.coffee-script.helpers.merge)
- description and source-code
```javascript
merge = function (options, overrides) {
  return extend(extend({}, options), overrides);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.nameWhitespaceCharacter"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>nameWhitespaceCharacter (string)](#apidoc.element.coffee-script.helpers.nameWhitespaceCharacter)
- description and source-code
```javascript
nameWhitespaceCharacter = function (string) {
  switch (string) {
    case ' ':
      return 'space';
    case '\n':
      return 'newline';
    case '\r':
      return 'carriage return';
    case '\t':
      return 'tab';
    default:
      return string;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.repeat"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>repeat (str, n)](#apidoc.element.coffee-script.helpers.repeat)
- description and source-code
```javascript
repeat = function (str, n) {
  var res;
  res = '';
  while (n > 0) {
    if (n & 1) {
      res += str;
    }
    n >>>= 1;
    str += str;
  }
  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.some"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>some ()](#apidoc.element.coffee-script.helpers.some)
- description and source-code
```javascript
function some() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.starts"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>starts (string, literal, start)](#apidoc.element.coffee-script.helpers.starts)
- description and source-code
```javascript
starts = function (string, literal, start) {
  return literal === string.substr(start, literal.length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.throwSyntaxError"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>throwSyntaxError (message, location)](#apidoc.element.coffee-script.helpers.throwSyntaxError)
- description and source-code
```javascript
throwSyntaxError = function (message, location) {
  var error;
  error = new SyntaxError(message);
  error.location = location;
  error.toString = syntaxErrorToString;
  error.stack = error.toString();
  throw error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coffee-script.helpers.updateSyntaxError"></a>[function <span class="apidocSignatureSpan">coffee-script.helpers.</span>updateSyntaxError (error, code, filename)](#apidoc.element.coffee-script.helpers.updateSyntaxError)
- description and source-code
```javascript
updateSyntaxError = function (error, code, filename) {
  if (error.toString === syntaxErrorToString) {
    error.code || (error.code = code);
    error.filename || (error.filename = filename);
    error.stack = error.toString();
  }
  return error;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
