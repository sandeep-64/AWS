### Q: What is AWS Lambda?
A: AWS Lambda is a serverless computing service that:
- Runs code automatically in response to events
- Requires no server management from users
- Automatically scales based on workload
- Only charges for actual compute time used
- Handles infrastructure management automatically

<img width="757" alt="image" src="https://github.com/user-attachments/assets/cf2aa8a0-ef10-4f9e-a3e3-9ba933334e7d" />

### Q: What are the key features of AWS Lambda?
A: Key features include:
- Auto-scaling and high availability
- Serverless execution
- Pay-per-use pricing model
- Support for multiple programming languages (Python, Node.js, Java, C#, etc.)
- Integration with other AWS services
- Version control and deployment management
- Security through IAM integration

### Q: What programming languages does AWS Lambda support?
A: AWS Lambda supports:
- Python
- Node.js
- Java
- C#
- PowerShell
- Go

### Q: How does AWS Lambda pricing work?
A: AWS Lambda pricing is based on:
- Number of requests made to your functions
- Compute time consumed
- Memory allocated to the function
- Free tier includes:
  - 1 million free requests per month
  - 400,000 GB-seconds of compute time per month

### Q: What are common use cases for AWS Lambda?
A: Common use cases include:
- File processing (triggered by S3 events)
- Web applications
- IoT applications
- Real-time stream processing
- API endpoints
- Automated backups
- Log analysis

### Q: What are the limitations of AWS Lambda?
A: Key limitations include:
- Maximum execution time of 900 seconds (15 minutes)
- Limited temporary storage (512MB)
- Cold start latency
- Limited control over infrastructure
- Memory configuration ranges from 128MB to 10GB
- Vendor lock-in to AWS ecosystem

### Q: How can you trigger AWS Lambda functions?
A: Lambda functions can be triggered by:
- AWS services (S3, DynamoDB, API Gateway)
- HTTP endpoints
- Mobile applications
- CloudWatch Events
- SNS notifications
- SQS messages
- Custom applications

### Q: What are the best practices for using AWS Lambda?
A: Best practices include:
- Optimize function performance to minimize cold starts
- Implement proper error handling and retries
- Use appropriate memory allocation
- Follow security best practices with IAM roles
- Keep functions focused and small
- Use environment variables for configuration
- Implement proper monitoring and logging

### Q: What are the key benefits of using AWS Lambda?
A: Key benefits include:
- Zero server management
- Automatic scaling
- Cost efficiency (pay-per-use)
- High availability
- Built-in fault tolerance
- Easy integration with AWS services
- Reduced operational overhead

### Q: How do you monitor AWS Lambda functions?
A: Monitoring can be done through:
- AWS CloudWatch metrics
- CloudWatch Logs
- AWS X-Ray for tracing
- AWS Cost Explorer for cost analysis
- Custom metrics and logging
- Third-party monitoring tools
