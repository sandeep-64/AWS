### Q: What is a VPC?
A: A Virtual Private Cloud (VPC) is a secure, isolated private section of AWS cloud where you can launch AWS resources in a network that you define.

### Q: Why do we need VPC?
A: VPC is needed for network isolation, enhanced security, resource organization, preventing unauthorized access between applications, and creating separate environments for different projects/applications.

### Q: What are the main components of a VPC?
A: The main components are Internet Gateway (IGW), Subnets (Public and Private), Route Tables, Network ACLs (NACLs), Security Groups, and NAT Gateway.

### Q: What is an Internet Gateway?
A: It's a VPC component that allows communication between your VPC and the internet. It acts as a gateway or entry/exit point for traffic.

### Q: What's the difference between Public and Private subnets?
A: Public subnets can directly access the internet through Internet Gateway, while Private subnets have no direct internet access and are typically used for backend resources that shouldn't be directly accessible from the internet.

### Q: What is a NAT Gateway?
A: A NAT (Network Address Translation) Gateway allows resources in private subnets to access the internet while preventing inbound connections from the internet, providing one-way internet access.

### Q: What's the difference between Security Groups and NACLs?
A: Security Groups are instance-level firewalls that control inbound and outbound traffic at the instance level and are stateful. NACLs are subnet-level firewalls that are stateless and control traffic at the subnet level.

### Q: What is a Route Table?
A: A Route Table contains rules (routes) that determine where network traffic from your subnet is directed. Each subnet must be associated with a route table.

### Q: How do you secure resources in a VPC?
A: Resources can be secured by:
- Placing them in private subnets
- Configuring proper Security Group rules
- Setting up NACLs
- Using proper network segmentation
- Implementing least privilege access

### Q: What is VPC Flow Logs?
A: VPC Flow Logs is a feature that enables you to capture information about the IP traffic going to and from network interfaces in your VPC for monitoring and troubleshooting.

### Q: What are the best practices for VPC design?
A: Best practices include:
- Planning IP address ranges carefully
- Separating public and private resources
- Using private subnets for application servers
- Implementing proper security controls
- Enabling VPC Flow Logs for monitoring
- Using NAT Gateway for private subnet internet access
