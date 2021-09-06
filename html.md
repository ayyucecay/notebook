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

.note {
  font-size: 120%;              The class attribute is often used to point to a class name in a style sheet.
  color: red;                   The HTML class attribute specifies one or more class names for an element
}
`<div class="note">`















