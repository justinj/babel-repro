In node 0.10:
```
$ npm i
$ npm test
```
gives me
```
> babel-repro@1.0.0 test /Users/justin/dev/babel-repro
> mocha --compilers js:babel-core/register

/Users/justin/dev/babel-repro/src/file.js:9
var Foobar = class Foobar {
             ^^^^^
SyntaxError: Unexpected reserved word
    at exports.runInThisContext (vm.js:73:16)
    at Module._compile (module.js:443:25)
    at loader (/Users/justin/dev/babel-repro/node_modules/babel-register/lib/node.js:127:5)
    at Object.require.extensions.(anonymous function) [as .js] (/Users/justin/dev/babel-repro/node_modules/babel-register/lib/node.js:137:7)
    at Module.load (module.js:355:32)
    at Function.Module._load (module.js:310:12)
    at Module.require (module.js:365:17)
    at require (module.js:384:17)
    at Object.<anonymous> (/Users/justin/dev/babel-repro/test/test.js:3:13)
    at Module._compile (module.js:460:26)
    at loader (/Users/justin/dev/babel-repro/node_modules/babel-register/lib/node.js:127:5)
    at Object.require.extensions.(anonymous function) [as .js] (/Users/justin/dev/babel-repro/node_modules/babel-register/lib/node.js:137:7)
    at Module.load (module.js:355:32)
    at Function.Module._load (module.js:310:12)
    at Module.require (module.js:365:17)
    at require (module.js:384:17)
    at /Users/justin/dev/babel-repro/node_modules/mocha/lib/mocha.js:216:27
    at Array.forEach (native)
    at Mocha.loadFiles (/Users/justin/dev/babel-repro/node_modules/mocha/lib/mocha.js:213:14)
    at Mocha.run (/Users/justin/dev/babel-repro/node_modules/mocha/lib/mocha.js:453:10)
    at Object.<anonymous> (/Users/justin/dev/babel-repro/node_modules/mocha/bin/_mocha:393:18)
    at Module._compile (module.js:460:26)
    at Object.Module._extensions..js (module.js:478:10)
    at Module.load (module.js:355:32)
    at Function.Module._load (module.js:310:12)
    at Function.Module.runMain (module.js:501:10)
    at startup (node.js:129:16)
    at node.js:814:3
```
