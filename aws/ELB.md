## ELB

Elastic load balancer

managed load balancer by aws , integrates well with many services

3 types of load balancers

ALB - application load balancer , layer 7 - http ,https, websocket
NLB -  network load balancer - tcp, ip, udp
Gateway load balancer - Layer3 i.e network layer load balancer - IP

## Application load balancer

Application load balancer can forward the http requests to different target groups based on http query, path
different target groups allowed - EC2, ECS, labda, other IP..

gets fixed host name 
app servers in target group dont see client ip , will be set as header X-frowarded-for

to setup define security group to allow http traffic , define target group to forward trafic to, define health check endpoints ..

setup listener rules and their priorities to act upon those requests based on http parameter (host name, path, query, header...)


X-Forwarded-For - header fot gettingip address of end client