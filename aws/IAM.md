# IAM - Identtity and access management

Root user - user who created aws account - logs in via email password, best practice to setup MFA
create sub users for different domains in your organization

users - can be assigned to groups - groups can have policies


A policy is a json document  with fields - Version , Effect , Action , Resource, Condition

    - Version
    - Effect : allow , deny
    - Action : aws resource for e.g ec2:*
    - Resource : 
    - Condition :


IAM policies are global

IAM - Free to use - no charges, supports MFA , federation - you can uses organizations identity provider to define users in organization

IAM user - name/password for logging in to console , access keys - for programmatic acces to CLI and SDK

