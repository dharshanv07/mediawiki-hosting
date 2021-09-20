# mediawiki-hosting
This repo contains cloudformation and ansible scripts used for hosting mediawiki in aws
The architecture for the application is as provided below
![mediawiki-thoughtworks](https://user-images.githubusercontent.com/28534583/134063573-0b780af9-8b15-4bc9-b983-c8ab2f887626.jpg)
Media wiki server is hosted  in ec2 instances frontended with a load balancer. Maria DB is hosted on a seperate instance.

**Infrastructure Creation**
To execute the cloudformation stack for creating the infrastructure, copy the contents inside AWS folder to an s3 bucket and provide the s3 url for mediawiki-main.cfn.yml file in aws console for cloudformation stacks.

**Configuration Managment**
To run the ansible script to install necessary packages run main.yml present in ansible folder.
