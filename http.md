# HTTP Notes

HTTP(The Hypertext Transfer Protocol) is a TCP/IP based communication protocol, that is used to deliver data (HTML files, image files, query results, etc.) on the World Wide Web. 

- HTTP is connectionless
- HTTP is media independent
- HTTP is stateless

__Client:__
The HTTP client sends a request to the server in the form of a request method, URI, and protocol version, followed by a MIME-like message containing request modifiers, client information, and possible body content over a TCP/IP connection.

__Server:__
The HTTP server responds with a status line, including the message's protocol version and a success or error code, followed by a MIME-like message containing server information, entity meta information, and possible entity-body content.

HTTP makes use of the Uniform Resource Identifier (URI) to identify a given resource and to establish a connection. 
```html
- HTTP-message   = <Request> | <Response> ;
```

