# Amazon Elastic Compute Cloud (Amazon EC2)

EC2  - Physical servers(gues they are virtual) with hardware provisioned by aws
per second or per hour billing

## Configuration

Amazon machine image - AMI
    - operating system
    - root volume with other softwares installed
    - can convert an EC2 into AMI so that we can avoid repetive work

Instance Type

    naming convention - (instance affinity, generation, attribute).(instance size)
    e.g - c5n.xlarge

    instance affinity: general purpose(M), compute(C) , memory(R) , Storage(Ig), GPU(P), HPC(H) optimized types of instances 

Key pair

Network settings
    Default VPC , allows public internet access

Security Groups or firewalls: what traffic is allowed

Storage - optional additional storage

IAM - what role this EC2 instance is in - to access other resources


## Life Cycle

Pending
Running

Rebooting - os rebbot , ip address, dns name, instance store volumen retained , remains on same physical server 

Stop/Stop-hibernate -> Stopping, Stopped - You can stop and start an instance if it has an Amazon Elastic Block Store (Amazon EBS) volume as its root device , retains ip addresses , can be on new physical machine if restarted
Storage is charged  

Shutting down, terminated - instance store , ip are lost,

## Pricing

- on demand : per hour or per second billing for compute , no long term commitment
- Spot Instances : set limits on how much you pay per hour, aws provisions if spare compute is available , used when fault tolerant state less workloads 
- Savings Plans: 1 - 3 years , low cost compared to ondemand
- Reserved Instances : 
    - Standard Reserved Instances: just like savings plan - pay partially/fully upfront, 72% off on demand
    - Convertible Reserved Instances: 54% off ondemand prices
    - Scheduled Reserved Instances: time window based reservation
- Dedicated Host: your own physical server


## Resilience

For high availability deploy in multiple az , fronted by load balancer


## Auto scaling

EC2 instances can be part of auto scaling group

Launch templates
Auto scaling group
Scaling Policy