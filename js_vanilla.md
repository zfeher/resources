## Compatibility
- [Kangax ES6 compatibility table](http://kangax.github.io/compat-table/es6/)


## ES Proposals / Next
- [ES proposal: Shared memory and atomics](http://www.2ality.com/2017/01/shared-array-buffer.html)
- [Asyncing Feeling about JavaScript Generators](https://www.bignerdranch.com/blog/asyncing-feeling-about-javascript-generators/)
- [ES proposal: import()](http://www.2ality.com/2017/01/import-operator.html)
- [ES proposal: Rest/Spread Properties](http://www.2ality.com/2016/10/rest-spread-properties.html)
- Async/Await
  - [Tips for using async functions (ES2017)](http://www.2ality.com/2016/10/async-function-tips.html)
  - [Async functions - making promises friendly](https://developers.google.com/web/fundamentals/getting-started/primers/async-functions)
  - [ES7 async functions](https://jakearchibald.com/2014/es7-async-functions/)
  - [Async Functions Proposal](https://tc39.github.io/ecmascript-asyncawait/)
- [ES proposal: asynchronous iteration](http://www.2ality.com/2016/10/asynchronous-iteration.html)

### Related Libs
- [Babel: Async functions](https://babeljs.io/docs/plugins/syntax-async-functions/)


## Polyfills/Shims/Transpilers

### Notes
- How to use browser implementations of new syntax instead of Babel transformation?
  - Babel should not transform syntax when browser has implemented the syntax.
  - this depends on the target browsers and their versions :(
  - core-js can be used to non syntax polifilling

- How to use browser implementations of new syntax instead of TypeScript transformation?
  - tsc can be configured to target ES6 and use ES2015+ libs or not
  - core-js can be used to non syntax polifilling

### Related Libs

- [babel-preset-env](https://github.com/babel/babel-preset-env)
- [core.js](https://github.com/zloirock/core-js)
- [regenerator](https://github.com/facebook/regenerator)
- [babel-polyfill](http://babeljs.io/docs/usage/polyfill/) [core-js][regenerator]
- [Babel.js](https://babeljs.io)


## Tricks
- [Require Parameters for JavaScript Functions](https://davidwalsh.name/javascript-function-parameters)


## Arrow Function/Fat Arrow/=>
- [When 'not' to use arrow functions](https://rainsoft.io/when-not-to-use-arrow-functions-in-javascript/) [tip]


## Strings
- [4 New String Methods in ES6 that you should know](http://wesbos.com/new-es6-string-methods/)


## Arrays
- [Search JavaScript Arrays Efficiently with includes and indexOf](http://thenewcode.com/1152/Search-JavaScript-Arrays-Efficiently-with-includes-and-indexOf)


## Typed Arrays
- [Exploring JavaScript: Typed Arrays](https://codingbox.io/exploring-javascript-typed-arrays-c8fd4f8bd24f#.cotf6ljbp)


## Template Strings
- [Tagged Template Literals](http://wesbos.com/tagged-template-literals/)
- [Easy Creation of HTML with JavaScript’s Template Strings](http://wesbos.com/template-strings-html/)


## Proxies
- [Pitfall: not all objects can be proxied transparently](http://www.2ality.com/2016/11/proxying-builtins.html)

## Promises
- [Exploring ES6: Promises](http://exploringjs.com/es6/ch_promises.html)
- [Avoid callbacks in Node.js with Bluebird promises](http://www.applandeo.com/en/avoid-callbacks-nodejs-bluebird-promises/) [node]

### Related Libs
- [bluebird](http://bluebirdjs.com/docs/getting-started.html)


## Iterators
- [Exploring ES6: Iterators](http://exploringjs.com/es6/ch_iteration.html)


## Generators
- [A Practical Introduction to ES6 Generator Functions](http://thejsguy.com/2016/10/15/a-practical-introduction-to-es6-generator-functions.html)
- [Exploring ES6: Generators](http://exploringjs.com/es6/ch_generators.html)

### Related Libs
- [co](https://github.com/tj/co)
