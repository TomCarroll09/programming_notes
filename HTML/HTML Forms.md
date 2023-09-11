## Tags

```
<form></form>
```
Contains the form elements

-----
```
<input>
```
A form element.

-----
```
<button></button>
```
A button

----
```
<label></label>
```
Groups an input element and the element text

----

```
<fieldset></fieldset>
```
Groups related label and input elements in a web form.

----
```
<legend></legend>
```
Acts as a caption for the content in the fieldset element.

----

# Attributes

```
<form action="https://example.com">
</form>
```
Specifies where to send the form to, this example will send it to "example.com"

----
```
<input type="example"> Text_Here
```
Specifies what type of input it is.
Values can be:
* radio - a radio button
* text - a text box
* checkbox - a checkbox.

----
```
<input name="input_name_here">
```
represents data when submitted, the name attribute is the same in the associated input elements.

----
```
<input placeholder="Placeholder text here">
```
placeholder text (can help indicate what data should be entered)

----
```
<input required>
```
Indicates that the input is required.

----
```
<input id="input1">
```
used to identify specific HTML elements.

----
```
<input value="input-value">
```
contains the value of the data being submitted.

----
```
<input checked>
```
makes it checked by default.

----
```
<button action="submit">Submit</button>
```
Will make the button submit the form, this usually is the defualt behaviour but its best to not rely on it.

-------
```
<label for="element_id"></label>
```
Will prevent the need to wrap the label element around the input element. the value should be the elements id.

------
# Tips:
the name attribute is used when there are multiple options, but you only want to user to select one of them, this differentiates it from the “id” attribute.
When receiving the data, the value attribute and the name attribute will show up on the results.

# Syntax
------
### \<form>\</form>
```
<form>
  <label><input type="text" name="textbox1" value="text1" required placeholder="text box"> text box1</label>
  <fieldset>
    <legend>Radio-Buttons</legend>
    <label><input type="radio" value="option1" name="radio1" id="radio1" checked required> radio button1</label>
  </fieldset>
</form>
```
### \<input>
```
<input type="radio" name="input1" value="option2"> option 2
```

