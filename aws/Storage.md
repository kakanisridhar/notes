## EBS - elastic block store

Limited to single AZ

EBS volume types

    HDD
        st1 - frequently accessed data , 125gb - 16tb
        sc1 - less frequent low cost 
    SSD
        gp2
        gp3 - general purpose ssd, 1gb - 16tb, max 16000 iops for fee , 3000 iops in general
        io1 - 4gb - 16 tb , max 64k iops , 
        io2 block express - 256,000 IOPS/volume, 4gb - 64tb

    io2 can be attached to multiple Ec2 instances


## Instance store

Ephemeral storage attached to instance , high throuhput , if any application want exceptional throuhput this along with taking snapshots and storing elese where can be a solution

## Encryption
data is encrypted in transit and at rest
Can be encrypted using kms keys

if any volume is not encrypted , a snapshot can be taken which allows encryption and use the snapshot to write it to encrypted store

snapshots are used for moving data between AZ and regions

## Elastic file store

Network file storage
CMS, wordpress, data sharing, linux only
allows mutliple Ec2 instance to write to the store
Can span different AZ
Expensive compared to gp2
High througput - 10gps

can be regional or one zone specific( for dev mode cost reduction)

performance mode 
    general purpose
    max io 

Thorugh put mode - has to be chosen at creation time
    bursting
    provisioned
    elastic
Storage tier
    Standard
    Infrequent acces
    Archive

    implement life cycle policies to move storage to different tier


## Terminology

latency - time between ec2 request and storage response
IOPS - read and write operations per second
Throughput - measure of sequential reads per second  - measured in mb/per second