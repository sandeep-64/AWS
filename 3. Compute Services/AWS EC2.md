### Q: What is Amazon EC2?
A: Amazon EC2 (Elastic Cloud Compute) is a web service that provides resizable compute capacity in the cloud. It's a virtual server combining CPU, RAM, and disk resources that can be scaled up or down based on needs.

### Q: Why is it called "Elastic" Cloud Compute?
A: "Elastic" refers to the ability to scale resources up or down easily. Users can increase or decrease computing resources, storage, and memory based on their needs, and only pay for what they use.

### Q: What are the five main types of EC2 instances and their use cases?
A: The five main types of EC2 instances are:

1. General Purpose (T and M series)
   - Balanced CPU, memory, and networking
   - For: Web servers, dev environments, small databases
   - Example: t2.micro, m5.large

2. Compute Optimized (C series)
   - High CPU performance
   - For: Batch processing, gaming servers, ML inference
   - Example: c5.large

3. Memory Optimized (R and X series)
   - Large memory capacity
   - For: Large databases, real-time analytics, SAP HANA
   - Example: r6g.large

4. Storage Optimized (I, D, H series)
   - High disk I/O and throughput
   - For: Data warehousing, NoSQL databases, file systems
   - Example: i3.large

5. Accelerated Computing (P, G, F series)
   - GPU/FPGA enabled
   - For: Machine learning, graphics processing, scientific computing
   - Example: p3.2xlarge

### Q: What does each part of the EC2 instance name "c5n.xlarge" represent?

A: The EC2 instance name "c5n.xlarge" breaks down into three distinct parts:
This naming convention helps identify the instance's characteristics at a glance - in this case, it's a 5th generation compute-optimized instance with enhanced networking capabilities and extra-large size configuration.

1. Instance Family (c): Compute-optimized instance type
2. Generation (5): The 5th generation of this instance family
3. Attribute (n): Network-optimized capability
4. Instance Size (xlarge): The relative size/capacity of the instance


### Q: What are AWS Regions and why are they important?
A: AWS Regions are geographical locations where AWS has data centers. They're important for:
- Meeting data sovereignty requirements
- Reducing latency for users
- Ensuring compliance with local regulations
- Providing disaster recovery options

### Q: What is an Availability Zone?
A: An Availability Zone is an isolated location within an AWS Region that contains one or more data centers. Each Region has multiple AZs to provide redundancy and high availability for applications.

### Q: What is a key pair in EC2?
A: A key pair consists of a public key and a private key that are used to connect to an EC2 instance securely. The public key is stored on the instance, while the private key is kept by the user to authenticate SSH connections.

### Q: What is the free tier limit for EC2?
A: AWS Free Tier includes 750 hours per month of t2.micro instances (1 CPU, 1GB RAM) for one year. This equals running one instance 24/7 for the month, or multiple instances within the 750-hour limit.

### Q: How can you connect to an EC2 instance?
A: You can connect to an EC2 instance using SSH with the private key:
```bash
chmod 600 keyname.pem
ssh -i keyname.pem ubuntu@public-ip-address
```

### Q: What is a Security Group?
A: A Security Group acts as a virtual firewall for EC2 instances to control inbound and outbound traffic. It contains rules that determine which network traffic is allowed to reach the instance.

### Q: Why should you choose a specific region for your EC2 instance?
A: Region selection should be based on:
- Proximity to end users (to reduce latency)
- Compliance requirements
- Data sovereignty laws
- Cost (prices vary by region)
- Service availability

### Q: What happens to an EC2 instance when you stop it vs. terminate it?
A: When you stop an instance, it remains in your account and maintains its data, but you're not charged for compute time. When you terminate an instance, it's permanently deleted and all data is lost unless backed up.

### Q: What is the difference between public and private IP in EC2?
A: A public IP is accessible from the internet and changes when the instance is stopped/started. A private IP is used for internal communication within the VPC and remains constant throughout the instance's lifetime.

### Q: What is the minimum and maximum size of an EC2 instance?
A: The minimum size in free tier is t2.micro (1 CPU, 1GB RAM). The maximum size varies by instance type, but can go up to 448 vCPUs and 24,576 GiB of memory for memory-optimized instances.
