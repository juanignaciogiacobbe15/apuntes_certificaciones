# Internet Protocol(IP)
- IP -> An address that is assigned to a machine so that other machines can communicate each other.
- IPv4:
	- Standard address structure of four 'octets' containing numbers between 0 and 255 for each octet.
- IPv6:
	- Replacement for IPv4, contains a 128 bit hexadecimal number for addressing. 

# Transmission Control Protocol(TCP)
- Method with which all transactions between IP address are communicated.
- This protocol provides a mechanism that transmits and verifies that data traffic arrives at its destination and can be assembled again in its correct order.
	- It relies on the send and acknowledgement system with its data packets.
	- Each data packet contains a number indicating to the receiver how the data should be reassembled in a particular order.

# User Datagram Protocol(UDP)
- A stateless connection between two hosts.
- Data packets are sent to a destination without any verification that they were received. The side effect of this type of communication is that there is less network overhead than a TCP connection.
- Examples of use: network gaming, DNS, non-critical data, etc.

# Internet Control Message Protocol(ICMP)
- Intended for networking equipment such as routers, network switches, firewalls, and other devices to send error messages between themselves.
- Often used to query a network device to check its availability.
- Example commands that utilize ICMP are: ping, traceroute.

# IP Class Ranges

![](../img/Pasted%20image%2020240924085026.png)


# Network Mask
- Defines a logical network(called a subnet) that indicates the start and end of a range of IP addresses.
- Ranges:
	- Each address class range has an associated network and subnet mask.

# Private IP Address Ranges
- Addresses that are used for internal networks. Prevents the need for every host to have an IP address assigned to it from a central authority.
- Not publicly routable - Meaning they will only route within an internal network, not the internet.

![](../img/Pasted%20image%2020240924091357.png)

# Network Gateway and Broadcast Address

> [!NOTE] Network Gateway
> Destination where network traffic goes that has no other matching route or that is not intended for the local network.


> [!NOTE] Broadcast Address
> An IP address that is used to broadcast messages to all hosts on a particular network.

- Broadcast address end with the last octect containing the number 255.