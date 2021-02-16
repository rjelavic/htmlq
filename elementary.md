	01%
	02%
	03%
	04%
	05%
	06%
	07%
	08%
	09%
	10%
	11%
	12%
	13%
	14%
	15%
	16%
	17%
	18%
	19%
	20%
	21%
	22%
	23%
	24%
	25%
	26%
	27%
	28%
	29%
	30%
	31%
	32%
	33%
	34%
	35%
	36%
	37%
	38%
	39%
	40%
	41%
	42%
	43%
	44%
	45%
	46%
	47%
	48%
	49%
	50%
	51%
	52%
	53%
	54%
	55%
	56%
	57%
	58%
	59%
	60%
	61%
	62%
	63%
	64%
	65%
	66%
	67%
	68%
	69%
	70%
	71%
	72%
	73%
	74%
	75%
	76%
	77%
	78%
	79%
	80%
	81%
	82%
	83%
	84%
	85%
	86%
	87%
	88%
	89%
	90%
	91%
	92%
	93%
	94%
	95%
	96%
	97%
	98%
	99%
	100%


# Elementary

What kind of tags are there?

* opening and closing

`<div>asdf</div>`; What is the element's content?

* `asdf`

Opening tag?

* `<div>`

Closing tag?

* `</div>`

`<div>`?

* The browser turns it into `<div></div>`

Do all elements have opening and closing tags?

* Empty elements do not.

`<div id="a">asdf<br></div>`

What is the element's content?

* `asdf<br>`

`document.getElementById("a").innerHTML`?

* `asdf<br>`

`document.getElementById("a").textContent`?

* `asdf`

You create a document `a.html` which contains just the letter `a`, you open the browser and inspect the elements, what do you find?

* `<html><head></head><body>a</body></html>`

You change the content of the head element: `<head><title>a</title></head>`, what changes?

* The tab title visible in the browser used to be `a.html`, now it's `a`

Some common empty elements?

* `img`, `input`, `link`, `meta`

What is quirks mode?

* A browser mode where the layout emulates nonstandard behavior in Navigator 4 and Internet Explorer 5. This is essential in order to support websites that were built before the widespread adoption of web standards. 

What is almost standards mode?

* In almost standards mode, there are only a very small number of quirks implemented. 

What is full standards mode?

* The behavior is the one described by the HTML and CSS specifications. 

Why do HTML5 documents need to start with the document type declaration?

* Because of quirks.

What is the document type declaration for HTML5?

* `<!DOCTYPE html>`

What is the default character encoding for HTML5?

* UTF-8

You write a character `a` followed by three spaces, followed by `b` in `a.html`, what is displayed to the user?

* `a b`

You write a character `a` followed by a newline, followed by `b` in `a.html`, what is displayed to the user?

* `a b`

How to display the text `<br>` to the user?

* `&lt;br&gt;`
	* HTML entity.

What is non-breaking space?

* The line will not be wrapped at that point, just like it wouldn't be werapped in the middle of a word.

`<!-- a -->`?

* Comment node. In the HTML document tree there are also text nodes and element nodes.

		<pre>
		a
		b
		</pre>

* This:

		a
		b

`<pre><br></pre>`?

* The same as `<br>`, `pre` does not escape.

`a.com/#b`

* Immediately after the page is opened the browser scrolls to the element with id `b`.
	* Document fragment

---

* [MDN web docs on HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [W3C HTML5 specification](https://www.w3.org/TR/html52/)
