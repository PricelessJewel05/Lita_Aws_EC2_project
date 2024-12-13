# Lita_Aws_EC2_project
This Project documents the process of launching EC2 instance and deploying Apache Web Server on it.
# Configuration of a custom VPC
Credit goes to LITA who already configured the VPC with each component details below.
## VPC Creation
The VPC creation with CIDR block of 10.0.0.0/16 was done by LITA to house resources in the AWS environment. 
### subnets
public subnet with CIDR- 10.0.1.0/24 and private subnet with CIDR- 10.0.2.0/24 were created and distinctly named.
### internet gateway
Internet gateway was attached to a VPC. route table was assigned to a route destination of 0.0.0.0/0 with association to a public subnet.
### NACL
This was done to provide extra layer of security by attaching it to the public and private subnet with definition of inbound rule by allowing HTTP 80 and SSH 22 and outbound rules.
## Security Group
This security group was created with inbound rules to allow HTTP 80 and SSH 20 and outbound rule to allow traffic from anywhere.Below is details of the security group.                                                                          !{security group}(/Screenshot_20241212_005515_png)
## Launching EC2 instance with Apache Web Server
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
This was created to serve as a unique identifier of EC2 resource
Below is the key pair details.                                                                                            !{keypair}(/jewelkeypair.pem)
#### Editing of Network Settings
In this part, the auto-assign public IP was set to enable
#### Storage configuration
Amount of storage was set to remain at 8gb
#### Review of processes done in launching instance
Input data was checked to be correct from top to bottom
#### Final launching of instance
Instance was launched with 2/2 check pass seen after a few minutes of initializing. Instance status was seen to be running.Below is details of running instance.                                                                             !{instance}(/launchinstance.png)
## Connecting launched instance with Apache Web Server
The instance already launched and running was connected to the apache web server by clicking SSH security group.
Key pair was located in the folder location and was opened in a terminal. After this, necessary commands were written even as due steps were followed and the apache was successfully created eventually. Below is the apache test page evidence showing my EC2 public IP address.                                                
!{testpage}(/testpage.png)
## Documentation of Project
This was done on the repository created in GitHub account with the aid of README .
I ensured files were uploaded accordingly and correctly and thereafter,committing changes and updating README.
After the whole project was reviewed, I shared my GitHub Repository link address on my LMS account and submitted.
