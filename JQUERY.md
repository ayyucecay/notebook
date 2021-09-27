# JQUERY NOTES

Basic syntax is: $(selector).action()

__jQuery Selectors__

```html
$(document).ready(function(){
  $("button").click(function(){              When a user clicks on a button, all <p> elements will be hidden. This is id selector.
    $(".test").hide();                       This is class selector.
  });
});

```

__jQuery Event Methods__
```html
$("p").click(function(){
  $(this).hide();                             When a click event fires on a <p> element; hide the current <p> element.
});
```
- The dblclick() function is executed when the user double-clicks on the HTML element.
- The mouseenter() function is executed when the mouse pointer enters the HTML element.
- The mouseleave() function is executed when the mouse pointer leaves the HTML element.
- The mousedown() function is executed, when the left, middle or right mouse button is pressed down, while the mouse is over the HTML element.
- The mouseup() function is executed, when the left, middle or right mouse button is released, while the mouse is over the HTML element.
- The hover() method takes two functions and is a combination of the mouseenter() and mouseleave() methods. <br>
The first function is executed when the mouse enters the HTML element, and the second function is executed when the mouse leaves the HTML element.
- The focus() function is executed when the form field gets focus.
- The blur() function is executed when the form field loses focus.

 
