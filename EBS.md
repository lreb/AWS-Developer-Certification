### [Back to main readme](Readme.md)

high performance block storage service designed for use with Amazon Elastic Compute Cloud (EC2) for both throughput and transaction intensive workloads at any scale.

- You can change volume types, tune performance, or increase volume size without disrupting your critical applications, so you have cost-effective storage when you need it.
- Designed for mission-critical systems
- replicated within an Availability Zone (AZ) and can easily scale to petabytes of data
- use EBS Snapshots with automated lifecycle policies to back up your volumes in Amazon S3
- ensuring geographic protection of your data and business continuity.
- Options
	- SSD-backed: storage for transactional workloads, such as databases and boot volumes (performance depends primarily on IOPS)
		- io1
			- I/O-intensive NoSQL and relational databases
			- 4 gb to 16 tb
		- gp2
			- Boot volumes, low-latency interactive apps, dev & test
			- 1 gb to 16 tb
	- HDD-backed: storage for throughput intensive workloads, such as MapReduce and log processing (performance depends primarily on MB/s).
		- st1
			- Big data, data warehouses, log processing
			- 500 gb to 16 tb
		- sc1
			- Colder data requiring fewer scans per day
			- 50 gb to 16 tb
- you can use [Cloud watch](Cloudwatch.md)
- Amazon EBS is a block level storage service for use with Amazon EC2. Amazon EBS can deliver performance for workloads that require the lowest-latency access to data from a single EC2 instance.