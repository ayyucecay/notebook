# HTML Notes


`<body>` section's content will be displayed in a browser.

`<title>`section's content will be shown in the browser's title bar or in the page's tab.

`<!DOCTYPE html>` All HTML documents must start with a document type declaration

`<a href="https://www.w3schools.com">This is a link</a>` HTML links are defined

`<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">`  Images are defined. SRC is source file.

`<p>This is a <br> paragraph with a line break.</p>` `<br>` tag defines a line break.

`<p style="color:red;">This is a red paragraph.</p>` style attribute is used to add styles to an element, such as color, font, size, and more.

`<hr>` usually draws a horizontal line within the page to split the page.

`<p><small>This is some smaller text.</small></p>` `<small>` x and similar uses set the font size and thickness properties related to the appearance of the text.

`<address>` tag defines the contact information for the author/owner of a document or an article.

```html
<head>
<style>
body {background-color: powderblue;}          An internal CSS is defined in the `<head>` section of an HTML page, within a `<style>` element.
h1   {color: blue;}
p    {color: red;}
</style>
</head>
```

```html
<head>
  <link rel="stylesheet" href="styles.css">    An external style sheet, add a link to it in the `<head>` section of each HTML page
</head>
```

`<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>` target="_blank" to open the linked document in a new browser window or tab

`<button onclick="document.location='default.asp'">HTML Tutorial</button>`  HTML button as a link

`<a href="html_images.asp" target="_blank">HTML Images</a>`  HTML attribute to make the link open in a new window.

```html
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">          HTML <map> tag defines an image map.
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">              An image map is an image with clickable areas.    
  <area shape="circle" coords="337,300,44" alt="Coffee" href="coffee.htm">               The areas are defined with one or more <area> tags.
</map>
```

```html
<picture>
  <source srcset="img_avatar.png">
  <source srcset="img_girl.jpg">                                                          Defines a container for multiple image resources
  <img src="img_beatles.gif" alt="Beatles" style="width:auto;">
</picture>
```

```html
<table>
  <tr>                                `<table>`	Defines a table
    <th>Person 3</th>                 `<th>`	Defines a header cell in a table    
  </tr>                               `<tr>`	Defines a row in a table
  <tr>                                `<td>`	Defines a cell in a table
    <td>Linus</td>
  </tr>
</table>
```

`<li>`	Defines a list item

`<div>` element is a block-level and is often used as a container for other HTML elements.

```html
.note {
  font-size: 120%;              The class attribute is often used to point to a class name in a style sheet.
  color: red;                   The HTML class attribute specifies one or more class names for an element
}
`<div class="note">`
 ``` 

`<h1 id="myHeader">My Header</h1>`  The id attribute specifies a unique id for an HTML element. The value of the id attribute must be unique within the HTML document.

`<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>` An inline frame is used to embed another document within the current HTML document.

```html
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";           This JavaScript example writes "Hello JavaScript!" into an HTML element with id="demo":
</script>
 ``` 
 
 ```html
<meta charset="UTF-8">                                                   The <meta> element is typically used to specify the character set,
<meta name="description" content="Free Web tutorials">                   page description, keywords, author of the document, and viewport settings.
<meta name="keywords" content="HTML, CSS, JavaScript">       
<meta name="author" content="John Doe">
<meta name="viewport" content="width=device-width, initial-scale=1.0">    The viewport is the user's visible area of a web page.
                                                                          It varies with the device - it will be smaller on a mobile phone than on a computer screen.
 ``` 

 ```html
<nav> - Defines a set of navigation links
<section> - Defines a section in a document
<article> - Defines an independent, self-contained content
<aside> - Defines content aside from the content (like a sidebar)
<footer> - Defines a footer for a document or a section
 ``` 
 
 ```html
A semantic element clearly describes its meaning to both the browser and the developer.
Examples of non-semantic elements: <div> and <span> - Tells nothing about its content.
Examples of semantic elements: <form>, <table>, and <article> - Clearly defines its content.
 ``` 












