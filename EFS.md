# Amazon EFS Elastic File System

### [Back to main readme](Readme.md)

Amazon EFS is a regional service storing data within and across multiple Availability Zones (AZs) for high availability and durability. Amazon EC2 instances can access your file system across AZs, regions, and VPCs, while on-premises servers can access using AWS Direct Connect or AWS VPN.

With a few clicks in the AWS Management Console, you can create file systems that are accessible to Amazon EC2 instances via a file system interface (using standard operating system file I/O APIs) and support full file system access semantics (such as strong consistency and file locking).

- Types
	- Standard storage class
	- Infrenquent access storage class (EFS IA)
		- provides price/performance that's cost-optimized for files not accessed every day.
		- The EFS IA storage class costs only $0.025/GB-month*
		-  files not accessed according to the lifecycle policy you choose will be automatically and transparently moved into EFS IA

- Uses
	- Customers can use EFS to lift-and-shift existing enterprise applications to the AWS Cloud
	- Amazon EFS is a file storage service for use with Amazon EC2. Amazon EFS provides a file system interface, file system access semantics (such as strong consistency and file locking), and concurrently-accessible storage for up to thousands of Amazon EC2 instances.

-  compatible with all Linux-based AMIs for Amazon EC2