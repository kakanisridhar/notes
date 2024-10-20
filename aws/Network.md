## Networking

IPv4 address - 32 bits - 4 group of  8 bits
Classless Inter-Domain Routing  - CIDR notation is a compressed way of representing a range of IP addresses. e.g 192.168.1.0/24 indicating first 24 bits are fixed , last 8 are variable


[VPC] (vpc.md)
[Netowrk Security](NetworkSecurity.md)


## Elastic IP 

Ec2 instances get public and private ip which changes upon instance termination
Inorder to get a dedicated IP assignment users can buy Elastic IP and assgin it tp Ec2 instance



## Elastic Netwrok Interface

Logical component in VPC representing Virtual network card

primary pvt ipv4 , one or more secondary ipv4
one elastic ipv4 per pvt ipv4
one public ipv4
one or more security groups
MAC address

2 ENI Can be attached to same EC2 , so that IP and traffic can be moved to another EC2 

used in advanced use cases