# aws certified solution architect associate

Region - region in a country/continent
Availability Zone - in a region


##VPC - Virtual Private Cloud

logically isolate a network
internetwork with other organization#
elastic ip address
enable hybrid cloud
single tenant dedicated hardware

done at network layer

VPN
network ACL
Security Groups
Peering connections

AWS reserves 5 ip addresses per subnet
subnets do not span availability zones

###Security Groups

resource level traffic firewall - e.g instance, ELB,
Stateful - return traffic allowed

###Access control

### Subnets

public and private subnets
different cidr block for each
NAT gateway is required if private wants to be exposed to outside world

Internet gateway router gives access to public subnet
 
for load balancing you can create nat gateway instead of NAT(EC2 instance)

### Endpoints 

For connecting to amazon services like S3 we have to create endpoint to connect pvt subnets to S3    
