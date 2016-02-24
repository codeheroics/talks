
title: ECMAScript 2016, and beyond

output: index.html
style: style.css

--

# ECMAScript (in) 2016, and beyond
## JavaScript++
By Hugo Agbonon ([@codeheroics](http://twitter.com/codeheroics))

--

## We're talking about...

* JavaScript: Invented in 1995 by Brendan Eich
* ECMAScript: JavaScript's spec
* TC39: Working group responsible for ECMAScript

--

## ECMAScript 2015
* Previously known as ECMAScript 6
* Renamed after TC39 decided on annual releases
* LOTS of new stuff
* You probably use some features with [Babel](https://babeljs.io/) or Node v4+

--

## ECMAScript 2015 is...
<span style="font-size: 150%;">
Arrow functions,
let, const,
Proxies,
Maps, Sets,
Template literals,
Destructuring,
Rest parameters,
Default parameters,
Spread,
Generators,
Symbols,
Iterators,
Classes,
Modules,
Promises…
</span>

--

## ECMAScript 2016

Should be equally awesome, right?

<img src="images/excited.gif" />

--

## ECMAScript 2016

You've heard about it!

* "[ES7 Decorators](https://twitter.com/search?q=ES7%20decorators)" (`@parisjs`)
* "[ES7 async/await](https://twitter.com/search?q=ES7%20async)" (Kill all the callbacks!)
* "[ES7 Object Spread properties](https://twitter.com/search?q=ES7%20spread)" `{...this.props}`

--

## ECMAScript 2016

Really contains...
* Array.prototype.includes
* Exponentiation Operator \*\*

--

## ECMAScript 2016

<img src="images/meh.gif" height="500" />

--

## Actually, that's ok

The annual release schedule means smaller releases.

ES2016 is so small because only two features were at **maturity stage 4**

--

## Enter ECMAScript proposals

[https://github.com/tc39/ecma262#current-proposals](https://github.com/tc39/ecma262#current-proposals)

5 stages to determine a proposal's advance

--

## Stage 0
### Strawman

An new idea is proposed. It is added after a preliminary review.

`Map-Set.prototype.toJSON` are here

--

## Stage 1
### Proposal

* A "champion" (responsible for the proposal) is identified.
* TC39 is committed to work on this feature
* **Significant changes** can still happen

Decorators (`@connect`) are here
--

## Stage 2
### Draft

At this point, it is likely it will end up being in the release.
Modifications from here are incremental.

Object rest/spread properties (`{...this.props}`) are here.

--

## Stage 3
### Candidate

The feature and its implementation are mostly ready

Async functions (`async`/`await`) are here.
--

## Stage 4
### Finished

The feature is complete and will be present in the next ECMAScript spec release.

--

## We use Babel, who cares about releases!
### Be careful when using experimental features

[**Object.observe**, once depicted as a revolution](http://www.html5rocks.com/en/tutorials/es7/observe/), was at stage 2 when it got killed.

(And if you're wondering, [Babel will stop supporting them the second they're dropped](https://www.reddit.com/r/javascript/comments/466mjm/does_anyone_else_have_es7_in_production/d03eh4l))

--

## Beyond ES2016

Lots of great features are coming to JS.

It doesn't matter if they aren't in ES2016, they'll be there next year

You can use most of the shiny new stuff now... But be careful when you use experimental features

--

### Thank you!

<div class="author" style="margin-top: 30px;">
  <img src="images/thanks.gif" height=300 style="margin-bottom: 10px;">
  <h3>
    Me: <a href="http://twitter.com/codeheroics">@codeheroics</a>
  </h3>
  <h3>
    This: <a href="http://bit.ly/es2016-parisjs">bit.ly/es2016-parisjs</a>
  </h3>
</div>

--

### Cool links

* [https://github.com/tc39/ecma262#current-proposals](https://github.com/tc39/ecma262#current-proposals)
* [http://www.2ality.com/2016/01/ecmascript-2016.html](http://www.2ality.com/2016/01/ecmascript-2016.html)
* [http://www.2ality.com/2015/11/tc39-process.html](http://www.2ality.com/2015/11/tc39-process.html)
* [http://kangax.github.io/compat-table/es7/](http://kangax.github.io/compat-table/es7/)
