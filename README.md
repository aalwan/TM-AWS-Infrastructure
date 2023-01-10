# TM-AWS-Infrastructure

This repository consists of a YAML template intended for the automated provisioning and configuration of Thought Machine's Vault into AWS. This template deploys a VPC, with a pair of public and private subnets spread across two Availability Zones. It deploys an internet gateway, with a default route on the public subnets. It deploys a pair of NAT gateways (one in each AZ), and default routes for them in the private subnets. Additionally, it deploys EKS control plane and worker node resources to run the microservices that make up Vault. Lastly, it deploys a PostgreSQL RDS instance as the data store. 
A diagram illustrating this can be seen below:

![image](https://user-images.githubusercontent.com/83315113/211580004-82e65e1c-f765-4fb4-9360-a71c9273bf20.png)
