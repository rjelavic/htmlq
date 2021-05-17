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

# Interaction

How to set default focus on an input element?

* `<input type="text" autofocus>`
	* Text is the default type, but here it's explicitly set for the sake of clarity.

How to create a disabled input element?

* `<input type="text" disabled>`

How to create a text input element with a default value?

* `<input id="a" value="a">`

Say you now write `b` into that input. `document.getElementById("a").getAttribute("value")`?

* `a`. The initial value is retuend (the same as when you inspect the HTML source code). Not the same thing as the current node property.

`$("#a").attr("value")`?

* `a`

`document.getElementById("a").value`? 

* `b`. Node property

`$("#a").prop("value")`?

* `b`

`$("#a").val()`

* `b`

How to set an input's value using js?

* `document.getElementById("a").value = "c"`
* `$("#a").prop("value", "d")`
* `$("#a").val("d")`

How to create a text input element with suggested values?

* `<input list="a"><datalist id="a"><option>b</option><option>c</option></datalist>`

Checkbox?

* `<input type="checkbox">`

Is it checked by default?

* No.

How to create a checked checkbox?

* `<input type="checkbox" checked>`

How to see if a checkbox is checked using js?

* `document.getElementById("b").checked`
* `$("#b").prop("checked")`

How to set a checkbox to be checked using js?

* `document.getElementById("b").checked = true`
* `$("#b").prop("checked", true)`

`<input type="radio" value="a"><input type="radio" value="b">`

* You get two circles right next to each other with no text and once you select one of them you can't unselect it. Also you can select both of them.

		<input id="a" type="radio" value="a">
		<input id="b" type="radio" value="b">
		<label for="a">a</label>
		<label for="b">b</label>

?

* Something like `* * a b`

		<input id="a" type="radio" value="a">
		<label for="a">a</label>
		<br>
		<input id="b" type="radio" value="b">
		<label for="b">b</label>
		<br>

?

* Looks like it should but still both options can be selected and once selected they stay selected.

		<input id="a" type="radio" name="a" value="a">
		<label for="a">a</label>
		<br>
		<input id="b" type="radio" name="a" value="b">
		<label for="b">b</label>
		<br>

?

* Now only one option can be selected.

		<input id="a" type="radio" name="a" value="a">
		a
		<br>
		<input id="b" type="radio" name="a" value="b">
		b
		<br>

?

* Now when you click on `a` or `b` nothing happens. Also, on mouseover the mouse coursor changes into `auto` (CSS) as different from the `default` (CSS) cursor.

How to set a default option for radio buttons?

* Like this:

		<input id="a" type="radio" name="a" value="a">
		<label for="a">a</label>
		<br>
		<input id="b" type="radio" name="a" value="b" checked>
		<label for="b">b</label>
		<br>

...

How to get the value of a selected radio button using js?

* By using `getElementsByName`, like this:

		function radioValueByName(name) {
			var es = document.getElementsByName(name);
			for(var i = 0; i < es.length; i++){
				if(es[i].checked){
					return es[i].value;
				}
			}
		}

How to get the value of a selected radio button using jQ?

* `$("[name=a]:checked").val()`

`<label>a</label><input>`. What happens when you click on `a`?

* Nothing.

`<label for="a">a</label><input id="a">`. What happens when you click on `a`?

* The input is now in focus.

How to create a dropdown with a default value?

* This:

		<select id="a">
		  <option value="1" selected>One</option>
		  <option value="2">Two</option>
		</select>

How to get the selected dropdown value using js?

* `document.getElementById("a").value`
* `$("#a").val()`

How to set the selected dropdown value using js?

* `document.getElementById("a").value = "2"`
* `$("#a").val("2")`

...

		<select id="a" size="2">
		  <option value="1" selected>One</option>
		  <option value="2">Two</option>
		</select>

?

* Now instead of a dropdown a list is displayed.

...

		<select id="a" size="2" multiple>
		  <option value="1" selected>One</option>
		  <option value="2">Two</option>
		</select>

?

* By holding `ctrl` or `cmd` and clicking options, multiple can be selected. Also it can be done by holding the mouse pressed.

...

		<select id="c">
		  <option value="" selected hidden>Choose here</option>
		  <option value="1">One</option>
		  <option value="2">Two</option>
		</select>

?

* The option is displayed by default but when you click on the dropdown it is not available.

`<textarea id="d">d</textarea>`; `document.getElementById("d").value`?

* `"d"`

`$("#d").val()`?

* `"d"`

How to set the textarea value?

* `document.getElementById("d").value = "e"`
* `$("#d").val("e")`

`$("#d").text()`?

* The initial value.
