
title: node.mjs

output: index.html
style: style.css

--

# node.mjs
By Hugo Agbonon ([@codeheroics](http://twitter.com/codeheroics))

--

## We're talking about...

* node.js
* ECMAScript 2015

--

## node v6
* Supports 93% of ECMAScript 2015

--

## node v6
* Does not support ES Modules.

--

## Modules

**CommonJS**
```js
const fs = require('fs')
const { networkInterfaces } = require('os')
const msg = 'Hello'
module.exports = { msg }
```
**ES Modules**
```js
import fs from 'fs'
import { networkInterfaces } from 'os'
export const msg = 'Hello'
```

Seems simple to move from one to the other, right?

--

## Differences

* CommonJS modules can be conditionally required
* ES modules export [immutable bindings](http://www.2ality.com/2015/07/es6-module-exports.html)
* ES modules need to be exported from the top level of the module
* ES modules are the standard
* **ES modules are parsed differently**

--

## Parsing differences mean...

**The same code won't work the same way whether it's in an ES Module or a CommonJS Module**
* (As an app developer, you probably won't have to worry about that though, the differences are subtle)
* However...
--

## Since they work differently

* We need to know for sure if we're running a CommonJS module or a ES module.

--

## 4 constraints for that

* **Maximum interoperability**: Existing requires *must* continue to work with no changes
* **Poly-Packages**: Library authors shoud be able to create packages that work with new and old versions of Node
* **Agnostic Usage**: Apps don't need to know if the module they're using is an ES or a CommonJS Module
* **A Future Without Vestiges**: CommonJS should fade.

--

## How can it be done?

* Checking for `import` and `export` is not enough: You can have ES modules without those keywords

--

## Options

1. `'use module'`
1. myModuleName.mjs
1. Automatic Detection
1. Information in package.json

--

## Chosen Option

1. ~~`'use module'`~~
1. myModuleName.mjs
1. ~~Automatic Detection~~
1. ~~Information in package.json~~

[The current official node proposal is for .mjs](https://github.com/nodejs/node-eps/blob/master/002-es6-modules.md) (though it is a draft and the implementation hasn't started)

--

## But I'm already using modules with Babel without it!

* You're *writing* ES Modules
* You're *running* transpiled CommonJS Modules

--

## When?

![Alt text](images/tweet.png)

implementation hasn't started.
Maybe around node v10?

--

## Get ready for node.mjs

--

### Thank you!

<div class="author" style="margin-top: 30px;">
  <img src="images/thanks.gif" height=300 style="margin-bottom: 10px;">
  <h3>
    Me: <a href="http://twitter.com/codeheroics">@codeheroics</a>
    <small>(React/Node Freelance! Available soon! Talk to me!)</small>
  </h3>
  <h3>
    This: <a href="http://bit.ly/parismjs">bit.ly/parismjs</a> (links at the last slide)
  </h3>
</div>

--

### Cool links

* [Node.js Enhancement Proposal](https://github.com/nodejs/node-eps/blob/master/002-es6-modules.md)
* [In Defense of .js](https://github.com/dherman/defense-of-dot-js/blob/master/proposal.md)
* [ES6 Module Detection in Node](https://github.com/nodejs/node/wiki/ES6-Module-Detection-in-Node)
* [Understanding the hard choice](https://medium.com/@bradleymeck/understanding-the-hard-choice-1ea3008fc9d0#.nsyo388o4)
* [https://twitter.com/nodemjs](https://twitter.com/nodemjs)
