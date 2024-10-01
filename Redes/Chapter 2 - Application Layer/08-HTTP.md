# HyperText Transfer Protocol(HTTP)
- Is the heart of the Web. HTTP defines how Web Clients request Web pages from Web Servers and how servers transfer Web pages to Clients.
- A Web page(also called a document) consists of objects. An object is simply a file that is addressable by a single URL.
- Most Web pages consist of a base HTML file and several referenced objects.
- Uses TCP as its underlying transport protocol. The HTTP client first iniciate TCP connection with the server. Once the connection is established, the browser and the server processes access TCP through their socket interfaces.
- HTTP need not worry about lost data or the details of how TCP recovers from loss or reordering of data within the network.
- The server send requested files to clients without storing any state information about the client. It maintains no information about the clients -> HTTP is a stateless protocol.