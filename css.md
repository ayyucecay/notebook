# CSS Notes

selector { property: value }        table{ border :1px solid #C00; }
-  A selector is an HTML tag at which a style will be applied. This could be any tag like `<h1>` or `<table>` etc.
-  A property is a type of attribute of HTML tag. Put simply, all the HTML attributes are converted into CSS properties. They could be color, border etc.
-  Values are assigned to properties. For example, color property can have value either red or #F1F1F1 etc.
```html
* { 
   color: #000000;         affects all elements
}
```
```html
.black {
   color: #000000;       All the elements having that class will be formatted according to the defined rule.
}
```
```html
h1.black {
   color: #000000;       Just h1 elements be black
}
```html
```
```html
#black {
   color: #000000;      All the elements having that id will be formatted according to the defined rule.
}
```
```html
<style type = "text/css" media = "all">
         body {
            background-color: linen;
         }
         h1 {                                           Put your CSS rules into an HTML document using the <style> element.
            color: maroon;                              This tag is placed inside the `<head>...</head>` tags.
            margin-left: 40px;
         }
      </style>
```
```html
<head>
   <link type = "text/css" href = "mystyle.css" media = " all" />    include style.css in any HTML document
</head>
```
```html
FONTS
style = "font-family:georgia,garamond,serif;"
style = "font-style:italic;"
style = "font-variant:small-caps;"                           demonstrates how to set the font variant of an element
style = "font-weight:bold;"
style = "font-size:20px;"                                    
style = "font-stretch:ultra-expanded;"                       demonstrates how to set the font stretch of an element
style = "font:italic small-caps bold 15px georgia;"          Shorthand Property
```
```html
TEXT
style = "color:red;"
style = "direction:rtl;"                                     demonstrates how to set the direction of a text. Possible values are ltr or rtl.
style = "letter-spacing:5px;"
style = "word-spacing:5px;"
style = "text-indent:1cm;"                                    
style = "text-align:right;"                                  demonstrates how to align a text. Possible values are left, right, center, justify.
style = "text-decoration:underline;"                         Possible values are none, underline, overline, line-through, blink.
style = "text-transform:capitalize;"                         Possible values are none, capitalize, uppercase, lowercase.
style = "white-space:pre;"                                   Possible values are normal, pre, nowrap.
style = "text-shadow:4px 4px 8px blue;"
```
```html
IMAGES
<img style = "border:0px;" src = "/css/images/logo.png" />
<img style = "border:1px solid red; height:100px;" src = "/css/images/logo.png" />
<img style = "border:1px solid red; width:150px;" src = "/css/images/logo.png" />
```
```html
LINKS
<style type = "text/css">
   a:link {color: #000000}
   a:visited {color: #006600}
   a:hover {color: #FFCC00}
   a:active {color: #FF00CC}
</style>
```
```html
-Border-collapse controls whether the edge of the other table is adjacent. Possible values: collapse, separate.
-The border-spacing specifies the width that should appear between table cells.
-The border-spacing property specifies the distance that separates adjacent cells'. borders. It can take either one or two values; these should be units of length.
-The caption-side property allows you to specify where the content of a <caption> element should be placed in relationship to the table.
-The empty-cells property indicates whether a cell without any content should have a border displayed.  Possible values: show, hide or inherit.
-The table-layout property is supposed to help you control how a browser should render or lay out a table.
```
```html
-The border-style specifies whether a border should be solid, dashed line, double line, or one of the other possible values.
-The border-width specifies the width of a border.
-Border-bottom-style changes the style of bottom border.
-The border-width property allows you to set the width of an element borders. Ex: border-bottom-width changes the width of bottom border.
-The border property allows you to specify color, style, and width of lines in one property. Ex: border:4px solid red;
```
```html
-The margin property defines the space around an HTML element. 
-The margin-bottom specifies the bottom margin of an element.
-The margin property allows you set all of the properties for the four margins in one declaration. Ex: margin: 10px 2% -10px; border:1px solid black;
```
```html
-The list-style-type allows you to control the shape or appearance of the marker. Ex: list-style-type:circle;
-The list-style-position specifies whether a long point that wraps to a second line should align with the first line or start underneath the start of the marker. Ex:list-style-position:inside;
-The list-style serves as shorthand for the preceding properties. Ex: list-style: inside square;
```
```html
-The padding property allows you to specify how much space should appear between the content of an element and its border.
-The padding-top specifies the top padding of an element.
-The padding serves as shorthand for the preceding properties. Ex: padding:10px 2%;
```
```html
`Overflow` which tells the browser what to do if the box's contents is larger than the box itself. Ex: overflow:scroll; 
```
