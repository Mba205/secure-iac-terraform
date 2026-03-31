# Secure Infrastructure as Code (Terraform)

This project provisions secure AWS infrastructure using Terraform.

It creates:
- A custom VPC
- A subnet
- A security group with restricted SSH access

The goal of this project is to demonstrate secure-by-default infrastructure design by defining cloud resources as code and limiting access to trusted sources only.

## Technologies Used

- Terraform
- AWS
- Infrastructure as Code (IaC)
- Network Security
- Cloud Security

## Resources Created

- `aws_vpc.main`
- `aws_subnet.public`
- `aws_security_group.secure_sg`

## Security Decisions

- SSH access is restricted to my public IP only
- Public IP auto-assignment is disabled in the subnet
- Infrastructure is defined and tracked as code

## Outputs

After deployment, Terraform returns:
- VPC ID
- Subnet ID
- Security Group ID

## How to Run

Initialize Terraform:

```bash
terraform.exe init
