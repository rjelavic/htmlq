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

# External

How to include CSS?

* `<link rel="stylesheet" href="my.css">`. 

Does the page load faster if `link` is in the `head` or on the bottom of the page?

* At the top, because so the elements need to be rendered only once.
	* Also, it is nicer since you avoid the _flash of unstyled content_.

How to include JS?

* `<script src="my.js"></script>`

What does the browser do until the script is downloaded?

* It waits.

In which order are the scripts executed?

* In that in which they are named.

`<script src="my.js" async></script>` What does the browser do now, until the script is downloaded?

* It continues parsing the document.

In which order are the scripts maked with `async` executed?

* In that order in which they are loaded.

What if one script depends on another and they are both `async`?

* Don't do that. The order of execution is not guaranteed.

`<script src="my.js" defer></script>` What does the browser do now, until the script is downloaded?

* It continues parsing the document.

In which order are the scripts marked with `defer` executed?

* In that in which they are named.

What if script X depends on script Y and they are both `defer`?

* Y needs to be referred to before X.

`<link rel="shortcut icon" href="favicon.ico" type="image/x-icon">`?

* Now the icon will be displayed in the browser tab and next to the bookmarked page.
