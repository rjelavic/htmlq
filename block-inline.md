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

# Block and Inline

What can the `display` CSS property be?

* `block`, `inline`, `inline-block`

`a<div>b</div>c`?

* This:

		a
		b
		c

* `div` is a block-level element (`display: block;`).

...

`a<span>b</span>c`?

* `abc`
* `span` is an inline element (`display: inline;`).
	* CSS height and width (and some other properties) are ignored.

`a<h6>b</h6>c`?

* This:

		a
		b
		c

...

`a<table></table>c`?

* This:

		a
		c

...

`a<li></li>c`?

* This:

		a
		*
		c

...

`a<img>b`?

* `ab`
* `display: inline-block;`
	* As opposed to `inline`, here CSS height, width (and some other properties) are not ignored, but still there is no newline before or after the element.

`a<em>b</em>c`?

* `abc`

`a<strong>b</stong>c`?

* `abc`

`a<ol>b</ol>c`?

* This:

		a
		b
		c

...

`a<ul>b</ul>c`?

* This:

		a
		b
		c

...

`a<a>b</a>c`?

* `abc`

`a<hr>b`?

* This:

		a
		---
		b

...

`a<input>b`?

* `a☐b`
* `display: inline-block;`

`a<button>b</button>c`?

* `abc`
* `display: inline-block;`
* same as `a<input type="button" value="b">c`

`a<label>b</label>c`?

* `abc`

`a<select>b</select>c`?

* `ac`
* `display: inline-block;`

`a<p>b</p>c`?

* This:

		a
		b
		c

Does `div` have margins around it by default?

* No.

Does `hr` have margins around it by default?

* Top and bottom.

Does `h1` have margins around it by default?

* Top and bottom.

Does a table have margins around it by default?

* No.

Do `ol` and `ul` have margins around them by default?

* Top and bottom.

Does `p` have margins around it by default?

* Top and bottom.

