# ec2-NGINX

This template will deploy an AWS EC2 instance with the following:
-NGINX Open Source AMI packaged by Bitnami (ami-0ed34781dc2ec3964)
-t2.micro instance type
-The key pair **nginx** will be assigned to the machine, 
-Security Group **NGINX-22-80-443** will be created and attached, opening ports 22, 80, and 443
-EBS volume of 250 GB
-File /opt/bitnami/nginx/html/index.html is modified at init to replace the standard greeting.
-Public IP will be an output of the CF stack

**USAGE**

Deploy an AWS CloudFormation stack using the cf-template.yml file. You can choose to change the instance type and AMI, or leave them as the default. 
