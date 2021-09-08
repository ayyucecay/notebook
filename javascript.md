# Javascript Notes
JavaScript is very easy to implement because it is integrated with HTML.

```html
<script language = "javascript" type = "text/javascript">
  <!--
  document.write("Hello World!")              JavaScript, anywhere within your web page, but it is normally recommended that you should keep it within the `<head>` tags.
//-->
</script>
```
```html
<script type = "text/javascript">
         <!--
            function sayHello() {
               alert("Hello World")         If you want to have a script run on some event, such as when a user clicks somewhere,
            }                                then you will place that script in the head as follows.
         //-->
      </script> 
```
```html
<body>
      <script type = "text/javascript">
         <!--
            document.write("Hello World")          If you need a script to run as the page loads so that the script generates content in the page,
         //-->                                     then the script goes in the <body> portion of the document. 
      </script>                                    In this case, you would not have any function defined using JavaScript.
      <p>This is web page body </p>
   </body>
```
```html
? : (Conditional )
If Condition is true? Then value X : Otherwise value Y

var a = 10;
var b = 20;
document.write ("((a > b) ? 100 : 200) => ");    
((a > b) ? 100 : 200) => 200 
```
```html
The typeof operator's value is a string indicating the data type of the operand.
```
```html
<script type = "text/javascript">
         <!--
            var age = 15;        
            if( age > 18 ) {
               document.write("<b>Qualifies for driving</b>");
            } else {
               document.write("<b>Does not qualify for driving</b>");
            }
         //-->
      </script>    
```
```html
for (aProperty in navigator) {
               document.write(aProperty);                    Try the following example to implement ‘for-in’ loop. It prints the web browser’s Navigator object.
               document.write("<br />");
            }    
```
```html
-onclick = "sayHello()"     This is the most frequently used event type which occurs when a user clicks the left button of his mouse.
-onsubmit = "return validate()"  This is an event that occurs when you try to submit a form. You can put your form validation against this event type.
-onmouseover = "over()"          event triggers when you bring your mouse over any element.
-onmouseout = "out()"            triggers when you move your mouse out from that element.
```
```html
Page Redirection

<script type = "text/javascript">
         <!--
            function Redirect() {
               window.location = "https://www.tutorialspoint.com";                         The implementations of Page-Redirection
            }            
            document.write("You will be redirected to main page in 10 sec.");              
            setTimeout('Redirect()', 10000);                                               This would need a bit time delay to load a new page.
         //-->
      </script>
```
```html
The JavaScript print function window.print() prints the current web page when executed.

<head>      
      <script type = "text/javascript">
         <!--
         //-->
      </script>
   </head> 
   <body>      
      <form>
         <input type = "button" value = "Print" onclick = "window.print()" />
      </form>   
   </body>

```


