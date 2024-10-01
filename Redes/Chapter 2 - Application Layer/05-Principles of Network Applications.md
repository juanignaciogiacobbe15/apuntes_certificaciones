# Principles of Network Applications
- You don't need to write software that runs on network-core devices, such as routers or link-layer switches.
- Application's architecture is distinctly different from the network architecture.
- The application architecture is designed by the application developer and dictates how the application is structured over the various end systems.
- A network application consists of pairs of processes that send messages to each other over a network.
- The process that initiates the communication is labeled as the client. The process that waits to be contacted to begin the session is the server.

## Client-Server Architecture
- **Server**: Always-on host. Has a fixed, well-known address, called an IP address.
- **Client**: The clients don't directly communicate with each other.
- A single-server host is incapable of keeping up with all the request from clients. -> The **data centers**(they house a large number of hosts) are often used to create a powerful virtual server.

## P2P Architecture
- There is minimal reliance on dedicated servers in data centers.
- The application exploits direct communication between pairs of intermittenly connected hosts, called *peers*.
- **Self-Scalability**: Each peer adds service capacity to the system by distributing files to other peers.
- Are cost effective, since they normally won't require significant server infrastructure and server band-width.
- P2P applications face challenges of security, performance and reliability fue to their highly decentralized structure.

## Processes Communicating
- Process: Program that is running within an end system.
- When processes are running on the same end system, they can communicate with each other with interprocess communication, using rules that are governed by the end system's operating system.
- Processes on two different end systems communicate with each other by exchanging messages across the computer network. A sending process creates and send messages into the network. A receiving process receives these messages and possibly responds by sending messages back.