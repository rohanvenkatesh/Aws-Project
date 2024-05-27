# Aws-Project
About the Project
In this Project i have demostrated how to create a VPC that you can use for servers in a production environment.

To improve resiliency, you deploy the servers in two Availability Zones, by using an Auto Scaling group and an Application Load Balancer. For additional security, you deploy the servers in private subnets.

The servers receive requests through the load balancer. The servers can connect to the internet by using a NAT gateway. To improve resiliency, you deploy the NAT gateway in both Availability Zones.

AWS Services used in the Project :
1.VPC (Virtual Private Cloud)

2.Auto Scaling Group

3.Application Load Balancer

4.EC2

5.NAT Gateway

6.Security Groups

7.Bastion Host / Jump Host

Detailed Insight of Project
Design and configure a VPC: Create a VPC with custom IP ranges. Set up public and private subnets. Configure route tables and associate subnets.

Implement network security: Set up network access control lists (ACLs) to control inbound and outbound traffic. Configure security groups for EC2 instances to allow specific ports and protocols.

Provision EC2 instances: Launch EC2 instances in both the public and private subnets. Configure security groups for the instances to allow necessary traffic. Create and assign IAM roles to the instances with appropriate permissions.

Networking and routing: Set up an internet gateway to allow internet access for instances in the public subnet. Configure NAT gateway or NAT instance to enable outbound internet access for instances in the private subnet. Create appropriate route tables and associate them with the subnets.

SSH key pair and access control: Generate an SSH key pair and securely store the private key. Configure the instances to allow SSH access only with the generated key pair. Implement IAM policies and roles to control access and permissions to AWS resources.

Test and validate the setup: SSH into the EC2 instances using the private key and verify connectivity. Test network connectivity between instances in different subnets. Validate security group rules and network ACL settings.

Results
✅Leveraged public and private subnets to create a secure environment with controlled access to resources. 🏢🔐

✅Implemented Auto Scaling groups to dynamically adjust server capacity based on demand, optimizing performance and cost efficiency. ⚖💻

✅Deployed Application Load Balancers to distribute incoming traffic across application servers, improving performance and availability. 🌐⚙

✅Implemented NAT gateways in each Availability Zone for secure internet access from private subnets. 🌐🔒

My Learnings & Key-Takeaways
By implementing this project, I have gained hands-on experience :

In setting up a secure VPC with EC2 instances.
Implementing networking and routing techniques.
Configuring security groups and IAM roles to ensure proper access control.
This project has helped me to develop a practical understanding of how these AWS services work together to create a secure and scalable infrastructure for my applications.
