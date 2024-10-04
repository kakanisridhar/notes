# Network Security

Network security in AWS is done by configuring Network Access Control list at network level and Security Groups at compute level


## Security groups 

By default allow only outbound traffic
So we have to configure ports to allow inbound traffic in the security group

security groups are stateful. That means that they will remember if a connection is originally initiated by the EC2 instance or from the outside, and temporarily allow traffic to respond without modifying the inbound rules.

In a 3 tier application architecutre , we have to create 3 security groups to allow source of traffic from above tier web -> app -> db

## Network Access Control List

Configure NACL if you want to fine tune what all trafic is allowed to VPC/subnet
By default it allows all traffic
Configure inbound and outbound rules to allow what ports are open

can be thought as Firewalls at the subnet level