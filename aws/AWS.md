# AWS
AWS - Infrastructure as service

Multiple regions, Multiple availability zones within a region and multiple Data centers within a zone

How to chose a region
	- Compliance : many countries and organizations have restrictions on where data can reside
	- Latency : Better to choose where your user base is
	- Pricing : pricing will be different for different regions within same continent
	- Service Availability: Not all services will be available in all regions 

Edge locations
	- Global locations where content is cached, Amazon CloudFront can distribute content to 400+ edge locations so that it will be served from the location closer to user
	

interaction with AWS services - via api calls - aws management console - web ui , aws cli , aws sdks

# Security 
Both you and AWS responsible for security

AWS responsibility: AWS for security of the cloud, i.e buildings and fiber cables, physical infra like virtualization servers , software.

Customer responsibility: you are responsible for patching os of ec2 instance , encrypting data in transit and rest, backing up data, configuring firewals.. 