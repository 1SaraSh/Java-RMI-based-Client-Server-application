# Java RMI Book Database

This project is a simple implementation of a client/server application using Java RMI. The server maintains a database of books, which can be accessed by multiple clients. Clients can add books to the database, retrieve information about specific books, or retrieve information about all books in the database.<br><br>



<h3>Classes and Interfaces</h3>
The project includes four classes and one interface:<br>
<ul>
          <li>
          <b>Book</b> class: This class defines the attributes of a book, including the title, author  name, and ISBN.
          </li>
          <li>
          <b>Communication</b> interface: This interface declares three methods that can be called by clients to interact with the server.<br>
          <li><b>addBook</b>: Takes three attributes (title, authorName, and ISBN) and adds a book to the database.</li>
          <li><b>getBook</b>: Takes one attribute and returns the corresponding Book object from the database.</li>
          <li><b>getAllBooks</b>: Returns a java.util.Map<String, Book> object containing all books in the database.</li>
          <li><b>Server</b> class: This class implements the <b>Communication</b> interface and all its methods. The server maintains the book database as a <b>java.util.Map<String, Book></b> object.</li>
          <li><b>Client</b> class: This class interacts with the server by calling the methods defined in the <b>Communication</b> interface.</li>
          </li>
         
</ul>     <br> 

<h3>Usage</h3>
<p>
To run the program, follow these steps:<br>
<ol>
<li>Compile all the classes using the command: <code>javac *.java</code>.</li>
<li>Start the server by running the command: <code>rmiregistry &amp; java Server</code>.</li>
<li>Start one or more client programs by running the command: <code>java Client</code>.</li>
<li>The clients can then interact with the server by calling the methods defined in the Communication interface.</li>
</ol>
</p>
<br><br>
<h3>Output</h3>
<p>When the client programs are run, you will see output in the console indicating the success or failure of the remote method calls being executed on the server. This will demonstrate how the client and server are able to communicate with each other using Java RMI.</p>

<h3>Conclusion</h3>
<p>This project demonstrates a simple implementation of a client/server application using Java RMI. It shows how multiple clients can interact with a server to maintain a shared database of books. With this basic framework, you can build more complex applications that use Java RMI to implement remote method invocation.</p>

