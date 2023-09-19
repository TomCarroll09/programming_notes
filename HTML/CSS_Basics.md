#CSS Basics

##Syntax
``` css
element {
attribute: value;
}
```
or
``` css
.class-name {
attibute: value;
```
or
```
#idname {
attribute: value
}

To have multiple elements/classes/ids in a selector:
```
.classname, element, otherelement {
attribute: value;
}


##Attributes and values
``` css
text-align
```
Aligns the specified text.
```
text-align: center;
```
Aligns the text to the center.

-----
```
background-color
```
sets the color of the background
``` css
background-color: burlywood;
```


##Useful Tips
``` html
<style></style>
```
You can nest css code inside a html document with this tag.

-----
``` html
<link rel="stylesheet" href="styles.css">
```
Links a seperate css file in the html document.

------
``` html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```
Makes the styling look much better  on mobile.

-----
``` html
<div id="id" class="class">
</div>
```
A \<div> element is a generic container for styling purposes.
