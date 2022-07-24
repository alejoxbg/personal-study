HTTP or HyperTest Transfer Protocol

A client is device that every person uses and a server is a computer that contains the application

As a clietn we do a request to a server to bring us the applicaition, thats the use

Now thes tansfer is made by a request and a response

A resquest and a response looks like this

![[Pasted image 20220723172115.png]]

HTTP has some headers as Host, Accept-Lenguage in the request example, there are some little pices of information useful for the application

the method is the way that the request is made, GET, POST, PUT, DELETE, PATCH are some of them with the version

Response

When the server recive the information it will responce with HTTP with a responce, it has headers as the request and a body, this is the content of the application as a JSON or XML, There are some codes as 200 OK, thats the state of the response, 200 are ok, 400 are bad responce, 500 are some internal error, 300 are for redirection, 100 are informative
![[Pasted image 20220723172646.png]]

Also Date is for the datetime where the responce was, server is the application that distribute the response, las modified, ETag is a hash for the cache, Acept ranges is how the infromation is delivered to the client, content length is the lenght of the body and content type is the type of the content of the body

![[Pasted image 20220723172856.png]]

IP is the fundameltal protocol to find any device

TCP Transmision control protocol and UDP user data protocol is to  transsmit data by the IP.

TLS transport layer security to deliver the data in a safe way and DNS domain name system, to convert a IP to a Domain

Above every those is HTTP, by the use of every protocol HTTP can transmit info between the client and the server, then the web will have to use these information

The server send the HTML, CSS and JS to a client and the web browser interpret those files, The client send a request HTTP to the server to response to the client the data needed.




