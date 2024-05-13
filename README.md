# Deploying a WordPress Website on AWS

## Project Overview
This project involves hosting a WordPress website on AWS using the management console. Including different resources for enhanced reliability, scalability and security.
URL to my project: ([Cristina Gonzalez Marrero - WordPress Website on AWS](https://www.cristinawordpressproject.com/))

## Architecture
- **IAM User**: For security reasons, it is best practice not to use the root user but instead creating IAM User with the appropriate permissions.
- **Virtual Private Cloud (VPC)**: Configured with public and private subnets across two availability zones for enhanced fault tolerance.
- **Internet Gateway**: Facilitates connectivity between VPC instances and the wider Internet.
- **Availability Zones**: Leveraged to enhance system reliability and fault tolerance.
- **Subnets**: Utilised public subnets for infrastructure components like NAT Gateway and Application Load Balancer. Positioned web servers (EC2 instances) within private subnets for enhanced security.
- **NAT Gateway**: Allows instances in private subnets to access the Internet.
- **Security Groups**: Used security groups to manage traffic from and to the aws resources.  
- **EC2 Instance Connect Endpoint**: Implemented for secure connections to assets within both public and private subnets.  
- **Amazon Elastic File System (EFS)**: Used for shared file system.
- **Amazon Relational Database Service (RDS)**: Used for database hosting.
- **Web Servers (EC2 Instances)**: Hosted the WordPress website on EC2 Instances.
- **Application Load Balancer (ALB)**: Used for evenly distributing web traffic to an Auto Scaling Group of EC2 instances across multiple Availability Zones. 
- **Installed WordPress**
- **Route 53**: Registered the domain name and set up DNS records.
- **Certificate Manager**: Secures application communications via TLS certificates. 
- **Auto Scaling Group**: Automatically manages EC2 instances, ensuring website availability, scalability, fault tolerance, and elasticity.
- **Simple Notification Service (SNS)**: Configured to alert about activities within the Auto Scaling Group.

## Reference Diagram

<img src="2._Host_a_WordPress_Website_on_AWS.png" width="400">

## Contributors

- [Cristina Gonzalez Marrero](https://github.com/cristicristi7)
- Azeez Salu: Course Instructor on Aos Note, https://www.aosnote.com/
