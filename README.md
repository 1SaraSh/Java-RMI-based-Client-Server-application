# Java-RMI-based-Client-Server-application

This is based on Java RMI. It shows the application of client/server application where the client invokes methods implemented on server side using Java RMI method. Imagine the scenario where we have multiple clients that are interacting with a server. Data entry operators are entering details about books which are stored at server side in Java Map, which is a key, value paired data structure. The client can also ask the server about data related to specific book. Some time the clients may ask for the data about all books. The following are specific information about how to implement this scenario.

In this project, 3 classes will be implemented and an interface:
•	Book Class: This class will have the attribute of a book, with a title, authorName and ISBN.

•	Communication interface: 3 methods will be declared and accessed be the server, 

o	addBook, takes three attributes title, authorName and ISBN.
o	getBook, takes one attribute (ISBN) and it returned the object of Book class.
o	getAllBooks, returns the Java Map<String, Book> object.

•	Server Class: will implement the Communication interface and all its methods.
•	Client Class: This class will invoke/call all three the methods implemented on server.

