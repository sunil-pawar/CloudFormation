
Description
----------------------------------------------------------------------------------------------------------------
The project is about creating amazon instance including the network elements viz VPC, public subent, IG, route table etc. using ansible playbook and cloud formation template as inputIt also includes the ansible plabook and dyanmic inventory file. Which will configure httpd to be able to show the current time form the sevrer on the html page.

-----------------------------------------------------------------
Files
-----------------------------

1. webservice.yaml --> cloud formation template
2. deploy_cloudform.yml --> playbook to create the cloudform stack
3. deploy_now.yml --> configure the httpd on instance to display current time of the instacne
4. test_aws_ec2.yml--> inventory file to be given as input to run the playbook -- deploy_now.yml
5. action_httpd_now.yml--> github action to run the playbook on self host
6. createinfraec2.yml--> github action to run playbook deploy_cloudform.yml

------------------------------------------------------------------------
Pre-Requisites
------------------------------------------------------------------------
1. Need an ansible server hosted on linux with boto3 and botocore  and configured to use python3 
2. Ansible file configured to use the aws_ec2 plugin
3. ansible file configured  to use the access key specified to access the instance in our case the filename is "ansible-node.pem"





