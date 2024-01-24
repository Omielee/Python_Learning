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

5. What are best practices when making the URI for RESTFul web-services?
- Develop them with understanding that forward flashes indicate hierarchy
- Use plural nouns for branches
- Use hyphens for multiple words
- Use lowercase
- Refrain from using file extensions

6. What are the differences between REST and SOAP?
- Definition
    - REST: Representational State transfer
    - SOAP: Simple object access protocal
- Nature
    - REST: an architecture to develop web services, flexible standards.
    - SOAP: a protocal for exchanging structure information by way of apis, standards are more strict in implementations, statefulness
- Data format
    - REST: Json, XML and others
    - SOAP: ONLY XML

7. What are the differences between REST and AJAX?
- Definition
    - REST: Representational State transfer, an architecture for handling HTTP requests
    - AJAX: asynchronous JavaScript and XML, a collection of web technologies that allow for asynchronous web application using the built-in xml HTTP Request object.
- REST API may handlie ajax clients and AJAX maybe used to send restful requests. BUT an api could never be implemented nor replaced by AJAX.

8. What are some tools used to develop and test REST APIs?
It depends. Node.js: Express. Test: postman

9. What are real-world examples of REST APIs?
When user get to the Amazon website, there is a get request sent to a server at the url for the necessary html to display to the user. 
For developers, restapis are used to manipulate data using the four main HTTP methods. 

**PROS**
- easy to learn
- wide range of data transfers
- statelessness
- scalability

**CONS**
- lack of built-in security
- need to be versioned for backward compatibility
- consistency in urls difficult to main for complex projects
