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

# Attributes

`<a href=#asdf></a>`?

* `<a href="#asdf"></a>`

`<a href='#asdf'></a>`?

* `<a href="#asdf"></a>`

`<a id="a"></a>`; `document.getElementById("a").getAttribute("href")`?

* `null`

`<a id="a" href></a>`; `document.getElementById("a").getAttribute("href")`?

* `""`

`<a id="a"></a href>`?

* `<a id="a"></a>`

`<input id="a" type="text" disabled="disabled">`; `document.getElementById("a").getAttribute("disabled")`?

* `"disabled"`
	* `disabled` is a boolean attribute.
* The input is disabled.

`<input id="a" type="text" disabled="">`; `document.getElementById("a").getAttribute("disabled")`?

* `""`
* The input is disabled.

`<input id="a" type="text" disabled>`; `document.getElementById("a").getAttribute("disabled")`?

* `""`
* The input is disabled.

`<input id="a" type="text" disabled="true">`; `document.getElementById("a").getAttribute("disabled")`?

* `"true"`
* The input now may or may not be disabled, depending on the browser.

`<input id="a" type="text">`; `document.getElementById("a").getAttribute("disabled")`?

* `null`
* The input is now not disabled.

Can you define arbitrary attributes?

* Yes. It is common to use `data-<arbitrary_name>` for storing data about elements.

...

		<div>a</div>
		<div hidden>b</div>
		<div>c</div>

?

* This:

		a
		c

...

		<div>a</div>
		<div style="display: none">b</div>
		<div>c</div>

?

* This:

		a
		c

...

		<div>a</div>
		<div style="visibility: hidden">b</div>
		<div>c</div>

?

* This:

		a
		
		c

...

`<span title="a">b</span>`?

* `b` is displayed but a tooltip with text `a` is displayed on mouseover.

What are HTML global attributes?

* Attributes which can be used on any HTML element. Examples: `id`, `class`, `title`, `style`, `hidden`.
