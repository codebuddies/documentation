### Coding Style Guide<a name="styleGuide"></a>
#### Standard JS - The Rules


* **2 spaces** - for indentation

* **Single quotes for strings** - except to avoid
escaping

* **No unused variables** - this one catches *tons* of bugs!

* **No semicolons** - [It's](http://blog.izs.me/post/2353458699/an-open-letter-to-javascript-leaders-regarding)
[ fine.](http://inimino.org/~inimino/blog/javascript_semicolons)
[ Really!](https://www.youtube.com/watch?v=gsfbh17Ax9I)

* **Never start a line with `(,[,` or `` ` ``!**
  * This is the **only** gotcha with omitting semicolons - * they are automatically checked for you!*
  * [More details](https://standardjs.com/rules-en.html#semicolons)

* **Space after keywords:** `if (condition) {...}`

* **Space after function name:** `function name (arg) { ... }`

* **Always use** `===` instead of `==`
 * The use of `obj == null` is allowed to check for `null || undefined`

* **Always handle** the `node.js err` function parameter

* **Always prefix** browser globals with `window`
  * Except for `document` and `navigator`, which are okay.
    * This prevents accidental use of poorly-named browser globals like `open, length, event,` and `name`.

* **And** [more goodness](https://standardjs.com/rules-en.html#javascript-standard-style) – *give `standard` a try today!*

To get a better idea, take a look at [a sample file](https://github.com/expressjs/body-parser/blob/master/index.js) written in JavaScript Standard Style. Or, check out one of the [thousands of projects](https://raw.githubusercontent.com/standard/standard-packages/master/all.json) that use `standard!`

>Courtesy of [StandardJS.com](https://standardjs.com/)</cite>

#### JavaScript Style Recommendations from [Meteor](https://guide.meteor.com/code-style.html#javascript)

<img src="https://guide.meteor.com/images/ben-es2015-demo.gif" alt="Refactoring">

> An example of refactoring from JavaScript to ES2015

##### Use the `ecmascript` package
ECMAScript, the language standard on which every browser’s JavaScript implementation is based, has moved to yearly standards releases... Meteor’s `ecmascript` package compiles this standard down to regular JavaScript that all browsers can understand using the popular Babel compiler. It’s fully backwards compatible to “regular” JavaScript, so you don’t have to use any new features if you don’t want to. We’ve put a lot of effort into making advanced browser features like source maps work great with this package, so that you can debug your code using your favorite developer tools without having to see any of the compiled output.

The `ecmascript` package is included in all new apps and packages by default, and compiles all files with the .js file extension automatically. See the [list of all ES2015 features supported by the ecmascript package](https://docs.meteor.com/packages/ecmascript.html#Supported-ES2015-Features).

To get the full experience, you should also use the `es5-shim` package which is included in all new apps by default. This means you can rely on runtime features like `Array#forEach` without worrying about which browsers support them.

##### Follow a JavaScript style guide

We recommend choosing and sticking to a JavaScript [style guide](#styleGuide) and enforcing it with tools.
