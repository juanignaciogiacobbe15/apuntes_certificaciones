# Amazon Elastic Compute Cloud(EC2)
- Provides secure, resizable compute capacity in the cloud as Amazon EC2 instances.
- When you're working with AWS, the servers are virtual, and the service you use to gain access to virtual servers is called EC2.
- Highly flexible, cost-effective and quick when you compare it to running your own servers on premises in a data center that you own.
- AWS took care of the hard part for you already. AWS already built and secured the data centers. AWS has already bought the servers, racked and stacked them, and they are already online ready to be used. AWS is constantly operating a massive amount of compute capacity. And you can use whatever portion of that capacity when you need it.
- Multitenancy: Sharing underlying hardware between Virtual Machines. EC2 runs on top of physical host machines managed by AWS using virtualization technology.
- The hypervisor is responsible for coordinating this multitenancy and it is managed by AWS. The hypervisor is responsible for isolating the virtual machines from each other as they share resources from the host.
- EC2 instances are also resizable.
- With an Amazon EC2 instance you can use a virtual server to run applications in the AWS Cloud.

	![[EC2_example.png]]

## EC2 Instance Types
- Each EC2 instance type is grouped under an instance family.
- They offer varying combinations of CPU, memory, storage and networking capacity.
- Types:
	- General purpose: balanced resources(compute, memory, and networking resources). Can be used for a variety of diverse workloads like web service or code repositories. For applications that does not require optimization in any single resource area.
	- Compute Optimized. Ideal for compute-intensive tasks like gaming servers, high performance computing or HPC, and even scientific modeling
	- Memory Optimized. Good for memory-intensive tasks. Memory optimized instances enable you to run workloads with high memory needs and receive great performance.
	- Accelerated Computing. Are good for floating point number calculations, graphics processing, or data pattern matching, as they use hardware accelerators.
	- Storage Optimized. For Workloads that require high performance for locally stored data.


## EC2 Purchase Options
- On-Demand. You only pay for the duration that your instance runs for.
- Savings plan: Offers low prices on EC2 usage in exchange for a commitment to a consistent amount of usage measured in dollars per hour for a one or three-year term.
- Reserved instances: There are suited for steady-state workloads or ones with predictable usage.
- Spot instances: They allow you to request spare Amazon EC2 computing capacity for up to 90% off of the On-Demand price. The catch here is that AWS can reclaim the instance at any time they need it, giving you a two-minute warning to finish up work and save state.
- Dedicated Hosts: Are physical hosts dedicated for your use for EC2. These are usually for meeting certain compliance requirements and nobody else will share tenancy of that host.

## Scaling EC2
> **Scalability** involves beginning with only the resources you need and designing your architecture to automatically respond to changing demand by scaling out or in.
-  You pay for only the resources you use. You don’t have to worry about a lack of computing capacity to meet your customers’ needs.

	![[scaling_ec2.png]]

- **Amazon EC2 Auto Scaling**: Automate scaling process. It enables you to automatically add or remove Amazon EC2 instances in response to changing application demand.
-  By automatically scaling your instances in and out as needed, you can maintain a greater sense of application availability.
- _Dynamic scaling_ responds to changing demand. 
- _Predictive scaling_ automatically schedules the right number of Amazon EC2 instances based on predicted demand.
- To scale faster, you can use dynamic scaling and predictive scaling together.
- You can add new instances to the application when necessary and terminate them when no longer needed.
- The **minimum capacity** is the number of Amazon EC2 instances that launch immediately after you have created the Auto Scaling group. In this example, the Auto Scaling group has a minimum capacity of one Amazon EC2 instance.
- **desired capacity** at two Amazon EC2 instances even though your application needs a minimum of a single Amazon EC2 instance to run.
- **Maximum capacity**. For example, you might configure the Auto Scaling group to scale out in response to increased demand, but only to a maximum of four Amazon EC2 instances.

	![[auto_scaling_group.png]]