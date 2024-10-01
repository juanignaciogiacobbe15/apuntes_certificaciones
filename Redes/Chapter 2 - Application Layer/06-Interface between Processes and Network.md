# Interface between Processes and Network
- Any message sent from one process to another must go through the underlying network.
- A process sends messages into, and receives messages from the network through a software interface called a **socket**.
- When a process wants to send a message to another process on another host, it shoves the message out of its door(socket). Once the message arrives at the destination host, the message passes through the receiving process's door(socket), and the receiving process then acts on the message.
- A socket is also referred to as the API between the application and the network, since the socket is the programming interface with which network applications are built.
- The application developer has control of everything on the application-layer side of the socket bus has little control of the transport-layer side of the socket.

## Addressing Processes
- The destination needs to have an address.
- In the [01-Internet](../Chapter%201%20-%20Computer%20Networks%20and%20Internet/01-Internet.md), the host is identified by its IP address.
- The IP address is a 32-bit quantity that we can think of as uniquely identifying the host.
- The sending process must also identify the receiving process running in the host. -> A destination **port number** serves this purpose.