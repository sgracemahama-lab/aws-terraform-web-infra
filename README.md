# AWS Terraform Web Infrastructure

This project creates a simple AWS web infrastructure using Terraform.

## What It Builds

- A Virtual Private Cloud (VPC) with public subnets
- An Internet Gateway for public internet access
- A Security Group allowing HTTP (80) and SSH (22) access
- An EC2 instance running Amazon Linux 2 with Apache web server

## How to Use

1. Configure your AWS credentials and default region (`us-east-1`).
2. Run Terraform commands:
terraform init
terraform validate
terraform plan
terraform apply

3. After apply, Terraform will output the public IP of the web server.
4. Open the public IP in your browser to see the Apache welcome page.

## Notes

- Replace the SSH ingress CIDR block in the security group with your own IP address plus `/32`.
- This is a basic example for learning Terraform and AWS fundamentals.

## Author

Created by Grace Mahama.
