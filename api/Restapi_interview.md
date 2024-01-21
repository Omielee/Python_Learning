1. How are REST APIs Stateless?
    
    In REST APIs, being stateless means that **each request from the client to the server must contain all the necessary information** for the server to understand and process it. The **server does not store** any state or session data about the client between requests. 

    This design ensures that each request is **independent**, and the server does not need to maintain or communicate any state information between subsequent requests. This approach **simplifies** the server design, improves scalability, and enhances the ability to distribute requests across multiple servers.

2. Explain the HTTP methods?
- Get: Read/Retrieve
- Post: Creat
- Put: Update
- Delete: Delete
CRUD

3. Explain the HTTP status codes?
- 200: a successful request and response 
- 400: a client-side error
- 500 : a server-side error

4. What is a URI?

   URI stands for uniform resource identifier，a standardized string that uniquely identifies a resource on the internet.
    
    It can be a **URL**, which locates and accesses resources like web pages or files, or a **URN**, which names a resource without describing its location. Essentially, a URI provides a universal way to reference any resource available in the network.

