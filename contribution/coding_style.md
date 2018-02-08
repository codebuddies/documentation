#### Coding Style Guide
# Standard JS - The Rules


* **2 spaces** - for identation

* **Single quotes for strings** - except to avoid
escaping

* **No unused variables** - this one catches *tons* of bugs!

* **No semicolons** - [It's](http://blog.izs.me/post/2353458699/an-open-letter-to-javascript-leaders-regarding)
[ fine.](http://inimino.org/~inimino/blog/javascript_semicolons)
[ Really!](https://www.youtube.com/watch?v=gsfbh17Ax9I)

* **Never start a line with `(,[,` or `` ` ``!**
  * This is the **only** gotcha with omitting semicolons - *automatically checked for you!*
  * [More details](https://standardjs.com/rules-en.html#semicolons)

* **Space after keywords:** `if (condition) {...}`

* **Space after function name:** `function name (arg) { ... }`

* **Always use** `===` instead of `==`
 * The use of `obj == null` is allowed to check for `null || undefined`

* **Always handle** the `node.js err` function parameter

* **Always prefix** browser globals with `window`
 * Except for `document` and `navigator`, which are okay.
   * This prevents accidental use of poorly-named browser globals like `open, length, event,` and
   `name`.

* **And** [more goodness](https://standardjs.com/rules-en.html#javascript-standard-style) – *give `standard` a try today!*

To get a better idea, take a look at [a sample file](https://github.com/expressjs/body-parser/blob/master/index.js) written in JavaScript Standard Style. Or, check out one of the [thousands of projects](https://raw.githubusercontent.com/standard/standard-packages/master/all.json) that use `standard!`

<cite> Courtesy of [StandardJS.com](https://standardjs.com/)</cite>
