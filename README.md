# Deploy-a-WordPress-Website-on-AWS
This project involves hosting a WordPress website on AWS using the management console. Including different resources for enhanced reliability, scalability and security.
URL to my project: ([Cristina Gonzalez Marrero](https://www.cristinawordpressproject.com/))

## Project Overview

The project utilises the following AWS resources:

0. **IAM User**:
   - For security reasons, it is best practice not to use the root user but instead creating IAM User with the appropriate permissions.

1. **Virtual Private Cloud (VPC)**:
   - Configured with public and private subnets across two availability zones for enhanced fault tolerance.
  
2. **Internet Gateway**:
   - Facilitates connectivity between VPC instances and the wider Internet.
  
3. **Availability Zones**:
   - Leveraged to enhance system reliability and fault tolerance.
  
4. **Subnets**:
   - Utilised public subnets for infrastructure components like NAT Gateway and Application Load Balancer.
   - Positioned web servers (EC2 instances) within private subnets for enhanced security.
  
5. **NAT Gateway**:
   - Allows instances in private subnets to access the Internet.
  
6. **Security Groups**:
   - Used security groups to manage traffic from and to the aws resources.
  
7. **EC2 Instance Connect Endpoint**:
   - Implemented for secure connections to assets within both public and private subnets.
  
8. **Amazon Elastic File System (EFS)**:
    - Used for shared file system.

9. **Amazon Relational Database Service (RDS)**:
    - Used for database hosting.

10. **Web Servers (EC2 Instances)**:
   - Hosted the WordPress website on EC2 Instances.

11. **Application Load Balancer (ALB)**:
   - Used for evenly distributing web traffic to an Auto Scaling Group of EC2 instances across multiple Availability Zones.
   
12. **Installed WordPress**

13. **Route 53**:
    - Registered the domain name and set up DNS records.

14. **Certificate Manager**:
    - Secures application communications via TLS certificates. 
   
15. **Auto Scaling Group**:
    - Automatically manages EC2 instances, ensuring website availability, scalability, fault tolerance, and elasticity.

16. **Simple Notification Service (SNS)**:
    - Configured to alert about activities within the Auto Scaling Group.


## Reference Diagram

![Reference Diagram](https://github.com/cristicristi7/Deploy-a-WordPress-Website-on-AWS/blob/main/2._Host_a_WordPress_Website_on_AWS.png)

## Contributors

- [Cristina Gonzalez Marrero](https://github.com/cristicristi7)
- Azeez Salu: Course Instructor on Aos Note, https://www.aosnote.com/
