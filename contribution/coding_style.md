#### Coding Style Guide
# Standard JS - The Rules


* **2 spaces** - for identation
<br>
* **Single quotes for strings** - except to avoid
escaping
<br>
* **No unused variables** - this one catches *tons* of bugs!
<br>
* **No semicolons** - [It's](http://blog.izs.me/post/2353458699/an-open-letter-to-javascript-leaders-regarding)
[ fine.](http://inimino.org/~inimino/blog/javascript_semicolons)
[ Really!](https://www.youtube.com/watch?v=gsfbh17Ax9I)
<br>
* **Never start a line with <span style="font-family: Courier">(,[, or `</span>**
  * This is the **only** gotcha with omitting semicolons - *automatically checked for you!*
  * [More details](https://standardjs.com/rules-en.html#semicolons)
<br>
* **Space after keywords:**
<span style="font-family: Courier">
<br>
&nbsp;&nbsp;if (condition) {...}
</span>
<br>
* **Space after function name:**
<span style="font-family: Courier">
<br>
&nbsp;&nbsp;function name (arg) { ... }
</span>
<br>
* **Always use** <span style="font-family: Courier">===</span> instead of <span style="font-family: Courier">==</span>
 * But <span style="font-family: Courier">obj == null</span> is allowed to check  <span style="font-family: Courier">null || undefined</span>.
<br>
* **Always handle** the <span style="font-family: Courier">node.js err</span> function parameter
<br>
* **Always prefix** browser globals with <span style="font-family: Courier">window</span>
 * Except <span style="font-family: Courier">document</span> and
  <span style="font-family: Courier">navigator</span> are okay.
   * Prevents accidental use of poorly-named browser globals like <span style="font-family: Courier">open, length, event,</span> and
   <span style="font-family: Courier">name</span>.
<br>
* **And** [more goodness](https://standardjs.com/rules-en.html#javascript-standard-style) – *give <span style="font-family: Courier">standard</span> a try today!*

To get a better idea, take a look at [a sample file](https://github.com/expressjs/body-parser/blob/master/index.js) written in JavaScript Standard Style. Or, check out one of the [thousands of projects](https://raw.githubusercontent.com/standard/standard-packages/master/all.json) that use <span style="font-family: Courier">standard!</span>

<cite> Courtesy of [StandardJS.com](https://standardjs.com/)</cite>
