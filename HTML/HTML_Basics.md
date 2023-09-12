# HTML Basics
## Elements

``` html
<!DOCTYPE html>
```
This is known as a declaration, it indicates that the document is a html5 document.

------
``` html
<html></html>
```
You nest all of your code inside these tags.

``` html
<html lang="en"></html>
```
Indicates webpage language. in this example the language is english (en)

-----
``` html
<head</head>
```
Contains meta-information about the document, the contents of the header is not displayed to the people viewing the web page.
``` html
<meta>
```
Sets browser behaviour
``` html
<meta charset="UTF-8">
<meta name+"viewport" content="width=device-width, initial-scale=1.0">
```
The first example, "charset" specifies the character set used in the document. the second example will make your website design more responsive(makes it look better on different devices)

-----
``` html
<title></title>
```
Sets the title viewed in the browser title bar.

------
``` html
<body></body>
```
Contains the parts of the webpage viewed by the user.

--------
``` html
<main></main>
```
Contains the main content of the webpage used to enhance SEO, amomg other things.

-----
``` html
<section></section>
```
Used to indicate a section of the web page.

-----
``` html
<p></p>
```
A paragraph element. can contain any text.

-----
``` html
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```
Different HTML headings, \<h1> is the largest heading and \<h6> is the smallest.

----
``` htnml
<img src="example.com/image.jpg" alt="image alt text">
```
Image tag, this one would contain the image "image.jpg" on example.com, and the alt text "image alt text".

-----
``` html
<a href="https://example.com" target="_blank">Link text</a>
```
Creates a link. in this example the link will bring you to "example.com" and it will open in a new tab(target="_blank").

-------
``` html
<!--Comment here-->
```
Comment, the comment in this example is "Comment here".

------
``` html
<figure>
  <img src="https://example.com/image.jpg" alt="example image">
  <figcaption>Example Image</figcaption>
</figure>
```
The \<figure> element is used to group images and captions together. The \<figcaption> element is the caption.

----
``` html
<hr>
```
Creates a horizontal line as a divider.

-----
``` html
<div></div>
```
A generic container used for styling purposes.

-----
``` html
<ol>
  <li>option1</li>
  <li>option2</li
  <li>option3</li>
</ol>
<ul>
  <li>option4</li>
  <li>option5</li>
  <li>option6</li>
</ul>
```
The \<ol> element is used to indicate an ordered (numbered) list. the \<ul> element is used to indicate an unordered (bulleted) list. \<li> is used to indicate a list item.

-----
```
