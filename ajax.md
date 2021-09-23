# AJAX Notes

AJAX just uses a combination of:

- A browser built-in XMLHttpRequest object (to request data from a web server)
- JavaScript and HTML DOM (to display or use the data)

## How AJAX Works

1. An event occurs in a web page (the page is loaded, a button is clicked)
2. An XMLHttpRequest object is created by JavaScript
3. The XMLHttpRequest object sends a request to a web server
4. The server processes the request
5. The server sends a response back to the web page
6. The response is read by JavaScript
7. Proper action (like page update) is performed by JavaScript

### XMLHttpRequest Object
- The XMLHttpRequest object can be used to exchange data with a server behind the scenes. This means that it is possible to update parts of a web page, without reloading the whole page.
- var xhttp = new XMLHttpRequest();

Send a Request To a Server
- To send a request to a server, use the open() and send() methods.
- xhttp.open("GET", "ajax_info.txt", true);<br>
  xhttp.send();<br>
  second parameter: url<br>
  third parameter: asynchronously <br>
  
  __The type of request: GET or POST__
  GET is simpler and faster than POST
  
   Use POST requests when:
    - A cached file is not an option
    - Sending a large amount of data to the server (POST has no size limitations).
    - Sending user input (which can contain unknown characters), POST is more robust and secure than GET.

- Server requests should be sent asynchronously.
- By sending asynchronously, the JavaScript does not have to wait for the server response

__The onreadystatechange Property__

With the XMLHttpRequest object you can define a function to be executed when the request receives an answer.

The function is defined in the onreadystatechange property of the XMLHttpResponse object
```html
    xhttp.onreadystatechange = function() {
  if (this.readyState == 4 && this.status == 200) {
    document.getElementById("demo").innerHTML = this.responseText;
  }
};
 ```
 - readyState property holds the status of the XMLHttpRequest.
 - status property and the statusText property holds the status of the XMLHttpRequest object.
 - When readyState is 4 and status is 200, the response is ready
 ### AJAX - Server Response
 __The responseXML Property__
 The responseXML property returns the server response as an XML DOM object.
 
 Using this property you can parse the response as an XML DOM object.
 ```html
xmlDoc = xhttp.responseXML;
txt = "";
x = xmlDoc.getElementsByTagName("ARTIST");
for (i = 0; i < x.length; i++) {
  txt += x[i].childNodes[0].nodeValue + "<br>";
  }
document.getElementById("demo").innerHTML = txt;
xhttp.open("GET", "cd_catalog.xml", true);
xhttp.send();
 ```
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
    
