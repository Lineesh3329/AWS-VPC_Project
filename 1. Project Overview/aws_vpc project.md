# AWS VPC PROJECT

This project demonstrates an AWS VPC architecture with public and private subnets across two Availability Zones. It includes NAT Gateway, Load Balancer, Auto Scaling, EC2 instances, and VPC for secure, scalable, and highly available cloud networking.

## AWS VPC Architecture Diagram

<img width="611" height="481" alt="image" src="https://github.com/user-attachments/assets/00baf132-53fb-4dc0-926b-46407ccd61d7" />

## Architecture Flow

- Public subnets contain NAT Gateways and Load Balancer
- Private subnets contain EC2 servers
- Load Balancer distributes traffic to servers
- Auto Scaling Group manages EC2 instances automatically
- NAT Gateway provides internet access for private servers
- Security Groups protect server access
- S3 Gateway Endpoint enables secure Amazon S3 connectivity

## Key Features

- High Availability using two Availability Zones
- Secure private subnet architecture
- Scalable infrastructure with Auto Scaling
- Controlled internet access using NAT Gateway
- Improved traffic distribution using Load Balancer

## Components Used

- VPC
- Public Subnets
- Private Subnets
- NAT Gateway
- Application Load Balancer
- Auto Scaling Group
- EC2 Servers
- Security Groups
- S3 Gateway Endpoint
