
# VPC - Virtual Private Cloud

logically isolate resources within AWS from external world & allow resources to interact
VPC is a network for your resources in AWS

network layer

## Configuration

CIDR block
name 
region

## Subnets

Subnets further divide the VPC so that accessiblity to network can be fine tuned

AWS reserves 5 ip addresses per subnet
subnets DO NOT span availability zones

### Subnet Configuration

VPC
name
CIDR range for the subnet which should be part of VPC cider range
Availability Zone

## Internet Gateway - IGW

Inernet gateway allows to connect recources in VPC to internet

how to create - create an IGW and attach it to VPC


## Virtual private Gateway - VGW

Allow connection from amazon to private network of your organization

## AWS direct connect

AWS direct connect service allows connection between AWS and private data center


## High availability

Since subnets dont span AZ, we need to duplicate subnets and compute resources in 2 AZ's


# Route Table

Route table define what interactions can be done by resources within the VPC/subnet and also what traffic can flow from outside

Main rout table which is created by default allows local traffic within VPC

You have to define a custom route table to allow traffic to flow from internet to IGW and associate subnets to which traffic from IGW can flow to.

You can protect your VPC by explicitly associating each new subnet with a custom route table and leaving the main route table in its original default state.


