# Getting started with AWS Identity And Access Management 
##### Follow the steps below to get started with the lab:

**1.Sign in to your AWS management Console:** Login to yous AWS Account using your credentials.

![alt text](SS/managamentconsolelogin.jpg)

**2.Login to the Account by entering the UserName/Email**

![alt text](SS/LoginPage.jpg)

**3.Continue by enter the password to complete the Signin**
![alt text](SS/Passowrd.jpg)

**4.Once the login is Successful You will be redirected to AWS Dashboard**
![alt text](SS/Dashboardservices.jpg)

___
# Introduction to AWS Identity And Access Management 
### LabDuration: 1 Hour
## Overview:
**What is IAM?**
AWS Identity and Access Management (IAM) is a web service that helps you securely control
access to AWS resources. With IAM, you can centrally manage permissions that control which AWS
resources users can access. You use IAM to control who is authenticated (signed in) and authorized
(has permissions) to use resources.
___

## Key Learnings:
In this hands-on lab, you will be learning the following:
* Understanding **AWS Identity And Access Management** Dashboard and its features
* Learn about differnt **Type of Policy**
* Create Customised Policies
* Learn to create **IAM users** and Managing IAM user by Policies
* Learn to create IAM groups and Adding Users into Groups
* Attaching **Inline policies** to IAM users and groups
* Deep-dive into understanding **Role** and Creating a Role 
___
## Hands-on Labs
* [Exercise 1:](#exploring-different-features-of-policy-and-there-types) Exploring Different Features of policy and there Types
* [Exercise 2](#exercise-2-creating-new-policy): Creating New Policy
* Exercise 3: Creating New Users and attaching Inline policy
* Exercise 4: Creating New Groups and Adding users to groups 
* Exercise 5: Creating Role For AWS services
___


# Exercise 1: Exploring Different Features of policy and there Types
This exercise will help you understand the concept of policy and various types of policies.

Policies are JSON documents in AWS that let you specify who has access to AWS resources, and what actions they can perform on those resources. You can attach a policy to an identity or resource to define their permissions. AWS evaluates these policies when the IAM principal makes a request. Permissions in the policies determine whether the request is allowed or denied.
**Different Types of Policies:**
* [AWS managed policy-Job function](#task-2-exploring-aws-managed-job-function-policies)
* [AWS managed Policy](#task-3-exploring-aws-managed-policies)
* [AWS Customer Policy](#task-1-creating-customer-managed-policies)

___

## Task 1: Exploring IAM Dashboard

1. To access the IAM dashboard via the AWS Dashboard, search "IAM" service in the search field.
![alt text](SS/IAMselect.jpg)
2. After selecting "IAM" service, you will be taken to the IAM Dashboard.
![alt text](SS/IAMdash.jpg)
___
## Task-2: Exploring AWS managed-job function Policies
**What are AWS managed- job function?**
AWS managed policies for job functions are designed to closely align with common job functions in the IT industry. These policies allow you to grant the necessary permissions to carry out tasks expected of someone in a specific job role.
1. Click on **Policies** under Access management in IAM dashboard.
![alt text](SS/policyclick.jpg)
2. Under **Filter by Type** dropdown Select for **AWS managed- job function**.
![alt text](SS/AWSmanaged-jobfunction.jpg)
3. Explore Different AWS managed- job function policies Pre-defined by AWS.
____
## Task 3: Exploring AWS managed Policies
**What are AWS managed policies?**
AWS managed policies are standalone policies that are created and administered by AWS1. They have their own ARNs that include the policy name. They are a collection of policies that make managing permissions as easy as possible2. They can be applied across the entire scope of specific AWS resources.

1.Under **Filter by Type** dropdown Select for **AWS managed**.
![alt text](SS/AWSmanaged.jpg)
2. Explore Different AWS managed policies Pre-defined by AWS.
___

# Exercise 2: Creating New Policy
## Task 1: Creating Customer managed policies:
**What are Customer managed Policies?**
A customer-managed policy is a critical component of AWS cloud security. It allows customers to define and enforce fine-grained permissions to access various AWS services and resources.
1.Click on **"Create policy"**
![alt text](SS/createpolicytoggle.jpg)
2.Select the **service** you intend to apply restrictions and set the policy editor to **Visual** for beginner-friendly operation.
![alt text](SS/createpolicyservice.jpg)
3.Select whether the policy should **allow or deny**.
![alt text](SS/EC2policyACtions.jpg)
4. Choose the actions to be performed.
![alt text](SS/denyruninstance.jpg)
5. Define the **resources**.
![alt text](SS/defineresources.jpg)
6. Conditions can be added to have fine grained restriction by clicking on **"Add another condition"**
![alt text](SS/Createanewcondition.jpg)
7. Select the apporiate values from the dropdows and enter the **Value**. Once complete click on **Add Condition**.
![alt text](SS/condition.jpg)
8. You can review the policy template by changing the policy editor to JSON.
![alt text](SS/JSON.jpg)
9. Click on **"next"** once the policy is defined.
![alt text](SS/policynextbutton.jpg)
10. Name the policy template under **"Policy Name"**.
![alt text](SS/policyname.jpg)
11. Click on **"Create policy"** once complete
![alt text](SS/createpolicyfinal.jpg)
____
Custom Policy can be reviewed under Filter by Type dropdown and selecting **"customer policy"**
___

# Exercise 3: Creating New Users and attaching Inline policy

An IAM user is an identity within your AWS account that has specific permissions for a single person or application. Users can be organized into groups that share the same permissions.
## Task 1: Creating IAM User



