# Amazon Virtual Private Cloud(Amazon VPC)
- Without boundaries around all of the resources that the clients created, network traffic would be able to flow between them unrestricted.
- Amazon VPC enables us to establish boundaries around AWS resources.
- Enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. Within a virtual private cloud (VPC), you can organize your resources into [[11-Subnets]]. 

## Internet gateway
-  Allow public traffic from the internet to access your VPC.
- Is a connection between a VPC and the internet. You can think of an internet gateway as being similar to a doorway that customers use to enter the coffee shop. Without an internet gateway, no one can access the resources within your VPC.

	![[internet_gateway.png]]

## Virtual Private Gateway
- Allows us to access private resources in a VPC.
- Is the component that allows protected internet traffic to enter into the VPC.
- Enables you to establish a virtual private network (VPN) connection between your VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC only if it is coming from an approved network.

	![[virtual_private_gateway.png]]

## AWS Direct Connect
- Establish a dedicated connection between the on-premises data center and the VPC.
- Is a service that lets you to establish a dedicated private connection between your data center and a VPC.
- The private connection that AWS Direct Connect provides helps you to reduce network costs and increase the amount of bandwidth that can travel through your network.

	![[aws_direct_connect.png]]