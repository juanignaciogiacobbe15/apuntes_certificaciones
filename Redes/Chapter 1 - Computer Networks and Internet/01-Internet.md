# Internet
> Is a computer network that interconnects billions of computing devices throughout the world. All of these devices are called **hosts or end systems**.
> Is an infrastructure that provides services to applications.
> Internet Standards: IETF standard documents are called Requests For Comments(RFCs).

- End systems are connected together by a network of **communication links and packet switches**
- Different links can transmit data at different rates, with the **transmission rate** of a link measured in bits/second.
- When one end system has data to send to another end system, the sending end system segments the data and adds header bytes to each segment.
- **Packets**: Are sent through the network to the destination end system, where they are reassembled into the original data.
- **Packet Switch**: Takes a packet arriving on one of its incoming communication links and forwards that packets on one of its outgoing communication links.
	- Link-layer switches are typically used in access networks.
	- Routers are typically used in the network core.
- Route or Path: The sequence of communication links and packet switches traversed by a packet from the sending end system to the receiving end system.
- End systems access the internet through Internet Service Providers(ISP). Each ISP is in itself a network of packets switches and communication links.
	- The ISPs that provide access to end end system must also be interconnected.

## A Services Description
- Applications are said to be distributed applications, since they involve multiple end systems that exchange data with each other.
- Internet applications runs on end systems: they do not run in the packet switches in the network core.
	- End systems are not concerned with the applications that is the source or sink of data.

### Socket Interface
- Provided by end systems attached to the Internet. It specifies how a program running on one end system asks the internet infrastructure to deliver data to a specific destination program running on another end system.
- Is a set of rules that the sending program must follow so that the internet can deliver data to the destination program.