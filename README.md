# aws_cloudformation_webserver

This is AWS CloudFormation template for installing an Apache webserver with "Hello World" static web page.

Assumptions
-----------
1. An AWS VPC alreday setup
2. Access to create CloudFormation stacks, EC2 instances, Security group etc
3. Existing SSH Key-pair
4. Existing public subnet

Installation
------------
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
In CloudFormation page Select the stack

Select Outputs tab 

Click on the URL. You should see Hello World page
