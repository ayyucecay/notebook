### API
- The API is the system that tells users how to get the necessary information from the systems they contact for information.

### REST
- APIs that follow REST principles are called.

__REST Architecture__
- It handles requests via HTTP.
- Stateless client-server communication ----> The server does not keep the requests made by the customer in memory. The customer submits his requests to the server in detail.
- Uniform interface. ----->The feature required for the interface between the client and the server to be developed independently of each other.
    - request must contain a single resource
    - the returning response should return with enough information because the client can edit it
    - every request should contain information that the server can understand, every response should contain information that the client can understand
    - Clients pass information in four different ways when making requests: Request body, query-string parameters, headers and URI. 
  The server does this in three different ways: response content, response code, and response header.
- Cacheable data. ------->The information must be storable. It is important for the client to create the cache.
- Client-server ------>The customer takes care of his own requirements. He takes care of his own work on the server. 
The server does not expect what will come from the client. If a request comes, he is interested in what comes.
Everyone does their own thing and doesn't care what the other is doing. The customer start communication.
- Layered system ------>not always the client sends a request to the server directly. 
 Certain structures can be found in between. In that case, each layer must communicate with the layer it is connected to.
- Code on demand -------> Sometimes the server wants to send executable code. Optional
