# Lita_Aws_EC2_project
This Project documents the process of launching EC2 instance and deploying Apache Web Server on it.
## vpc creation
The VPC creation with CIDR of 10.0.0.0/16 was done by LITA to house resources in the AWS environment
## Security Group
This security group was created with inbound rules to allow HTTP 80 and SSH 20 and outbound rule to allow traffic from anywhere.
Below is details of the security group
!{security group}(/Screenshot_20241212-005515.png)
## launching EC2 instance with Apache Web Server
