# aws_cloudformation_webserver

This is AWS CloudFormation template for installing an Apache webserver with "Automation for the People" static web page.

Assumptions
-----------
1. An AWS VPC already setup
2. Access to create CloudFormation stacks, EC2 instances, and Security group
3. Existing SSH Key-pair
4. Existing public subnet

Installation
------------
Click
<a href="https://console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/new?&templateURL=https://s3-us-west-2.amazonaws.com/shaimon-public-cf-templates/webserver.template" target="_blank"><img src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png"></a>  
###### OR follow these steps  
1. Login to AWS web console and click on CloudFormation  
2. Click on Create Stack  
3. Select Upload a template to Amazon S3 and click on Choose File  
4. Select webserver.json and click Next  
5. Type-in name of the stack in Stack name box  
6. Select KeyName  
7. Edit SSHLocation  
8. Select Subnet and VPC  
9. Click Next  
10. Click Next  
11. Click Create  

Validation
----------
* In CloudFormation page Select the stack  
* Select Outputs tab  
* Click on the URL. You should see a static page displaying "Automation for the People'
