# Simple Storage Service(S3)
- Object-Based Storage: Secure, durable, highly scalable object storage.
	- Manages data as objects rather than in file systems or data blocks.
	- Upload any file type.
	- Cannot be used to run an OS or DB.
- Scalable: Store and retrieve any amount of data from anywhere on the web at a very low cost.
	- The total volume of data and the number of objects you can store is unlimited.
	- S3 objects can range in size from a minimum of 0 Bytes to a maximum of 5 Terabytes.
	- Store files in buckets(similar to folders).
	- Scales automatically to meet demand. Many enterprises will put static websites on S3 when they think there is going to be a large number of requests.
- Simple: Easy to use, with a simple web service interface.
- Is a safe place to store your files: The data is spread across multiple devices and facilities to ensure availability and durability.
	- S3 is built for availability and designed for durability.
	- After a successful write of a new object(PUT) or an overwrite of an existing object, any subsequent read request immediately receives the latest version of the object.
	- Strong consistency for list operations, so after a write, you can immediately perfoam a listing of the objects in a bucket with all changes reflected.

## Working with S3 Buckets
- Universal Namespace: All AWS accounts share the S3 namespace. Each S3 bucket name is globally unique.

	![](../img/Pasted%20image%2020240905085822.png)

- Uploading files: When you upload a file to an S3 bucket, you will receive an HTTP 200 code if the upload was successful.


## Key-Value Store
- Key: The name of the object.
- Value: The data itself, which is made up of a sequence of Bytes.
- Version ID: Important for storing multiple versions of the same object.
- Metadata: Data about the data you are storing.


## S3 Standard
- High Availability and Durability. Data is stored redundantly across multiple devices in multiple facilities (>= 3 AZs).
- Designed for Frequent Access.
- Suitable for Most Workloads.
	- The default storage class.
	- Use cases include websites, content distribution, mobile and gaming applications, and big data analytics.

## Versioning Objects
- All versions of an object are stored in S3. This includes all writes and even if you delete an object.
- Can be a great Backup tool.
- Cannot Be Disabled.
- Lifecycle rules.
- Supports MFA.


que significa que un bucket sea publico?
Versioning se puede integrar con codeCommit?