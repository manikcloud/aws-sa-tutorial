# aws-sa-tutorial
Aws Solution-Architect-Tutorial 

# How to install Web-server

```
sudo yum install httpd -y

sudo service httpd start
sudo service httpd status

sudo /var/www/html/
sudo vim  /var/www/html/index.html

sudo chkconfig httpd on 
```
# instance meta-data

```

sudo curl http://169.254.169.254/latest/meta-data/public-ipv4
curl http://169.254.169.254/latest/
curl http://169.254.169.254/latest/meta-data
curl http://169.254.169.254/latest/meta-data/ami-id

```

# How to Create a VPC and its component

## Blog: https://varunmanik1.medium.com/how-to-create-aws-vpc-in-10-steps-less-than-5-min-a49ac12064aa

```
1.	Create vpc
2.	Create pub-subnet
3.	Create private-subnet
4.	Create IGW for pub subnet
a.	And attached to the VPC
5.	Create Public Route table 
a.	And attached the IGW with destination 0.0.0.0/0
b.	Associate the Public Subnet
6.	Create NAT gw for private subnet
a.	Create elastic ip 
7.	Create private Route table
a.	Attached Nat-GW
b.	Associate the Private Subnet

8.	Create DHCP Option Set
9.	Create EndPoint 

```
```
How to create Auto Scaling group and Launch Configuration 
from rohit_bargotra@yahoo.co.in to All Participants:
1.    Create an instance in a public subnet & connect 
2.    Update & Install the Apache 
3.    Start the service 4.    Insert the code in AWS CLI 
5.    Ensure correct port (Launch Wizard 1 – Inbound Rule – Add HTTP – Anywhere) 
6.    Create Image (Instance – Action – Image & template – Create AMI) 
7.    Create Launch Configuration (Name – AMI – Choose Instance type – IAM Role if any – root volume – security group – key pair – Create) 
8.    Create Auto Scaling Group (Name – select Launch configuration – Select VPC – Subnet – Load balancer – Health Check – Group Size – Capacity – Create Auto Scaling Group 
9.    Go to EC2 – Instances – Auto Scaling Groups must be initializing 
10.    Copy the Public IP and run it in the browser to verify

```
```
->create an instance ->connect with your instance ->make sure port http 80 should open. if not go to security group->inbound group and add HTTP porta 80 and select anywhere  ->install apache ->start service(service https start)-> start httpd.service->chkconfig httpd on ->vim /var/www/html/index.html ->paste & save your content -> :wq ->select and instance  ->click on action & select image and template  ->create a image ->select auto scaling & click launch configuration  ->give a name & select AMI ->select an existing key pair and click launch configuration  ->now select auto scaling groups & click on auto sclaing group ->give an name ->switch to auto scaling group ->select launch configuration and click on next ->choose instance launch options ->select vpc and AZ ->click on next ->select No balance loader ->click on next and select group size and scaling policies ->give desires,min,max capicity  ->click on next and click on auto scaling group ->now we can see all auto scaling groups in list view
```
# Varun's Blog
- https://varunmanik1.medium.com/a-simple-machine-learning-step-by-step-tutorial-with-the-help-of-amazon-translate-lambda-api-1cc200bf2212

# References

1. https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-add-user-data.html
2. https://aws.amazon.com/certification/certified-solutions-architect-associate/
3. https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/connecting_to_windows_instance.html
4. https://en.wikipedia.org/wiki/Hypervisor
5. https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-using-volumes.html
6. https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/recognize-expanded-volume-linux.html
7. https://www.w3schools.com/html/default.asp
