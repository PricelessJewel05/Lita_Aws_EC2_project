# Lita_Aws_EC2_project
This Project documents the process of launching EC2 instance and deploying Apache Web Server on it.
## vpc creation
The VPC creation with CIDR of 10.0.0.0/16 was done by LITA to house resources in the AWS environment
## Security Group
This security group was created with inbound rules to allow HTTP 80 and SSH 20 and outbound rule to allow traffic from anywhere.
Below is details of the security group
!{security group}(/Screenshot_20241212-005515.png)
## launching EC2 instance with Apache Web Server
An EC2 instance launch.
Below is each step taken
#### naming of instance
FoyinsolaAkinlosiwaju_lita
#### selection of Operating system
Amazon Linux 2
#### Instance type
t2.micro
#### selection of public subnet created by Lita
public subnet_Lita
#### creation of key pair
This was created to serve as a unique identifier of resources
Below is the key pair details
!{keypair details}(/JewelKeyPair.pem)
#### Editing of Network Settings
In this part, the auto-assign public IP is set to enable
#### Storage configuration
Amount of storage was set to remain at 8gb
#### Review of processes done in launching instance
Input information was checked to be correct from top to bottom
#### Final launching of instance
Instance was launched with 2/2 check pass seen after a few minutes of initializing. Instance status was seen to be running.
## Connecting launched instance with Apache Web Server
The instance already launched and running was connected to the apache web server by clicking SSH security group.
Key pair was located in the folder location and was opened in a terminal. After this, necessary commands were written even as due steps were followedband the apache was successfully created eventually. 
Below is the apache test page evidence showing my EC2 public IP address 
!{apache teatpage}(/Apachetestpagejpg)
