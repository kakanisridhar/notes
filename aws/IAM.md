# IAM - Identtity and access management

Root user - user who created aws account - logs in via email password, best practice to setup MFA
create sub users for different domains in your organization

users - can be assigned to groups, can be assigned policies
groups - can contain only users and policies

A policy is a json document  with fields - Version , Statement* - { Effect , Action , Resource, Condition }

    - Version
    - sid
    - Effect : allow , deny
    - Action : aws operations for e.g ec2:*
    - Resource :  resource and condition used in combination to define different type of allow deny criteria
    - Condition :


IAM policies are global

IAM - Free to use - no charges, supports MFA , federation - you can uses organizations identity provider to define users in organization

IAM user - name/password for logging in to console , access keys - for programmatic acces to CLI and SDK

## Programmatic access - IAM roles

IAM role - usually associated with an EC2 instance or lamda to programmatically aquire temporary credentials and make api calls on behalf of code

Identity providers uses IAM roles , users on IDP aquire federated roles to access resources
AWS IAM identity center is used for doing this

## Auditing security

IAM credential reports - for audting all users
IAM access advisor  - for finetuning policies at user/group level 


[Back to index](index.md)
