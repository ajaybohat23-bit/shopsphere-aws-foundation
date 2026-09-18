## Compute Infrastructure

### Bastion Host

A dedicated EC2 bastion host has been deployed in the public subnet for controlled administrative access.

| Property | Value |
|---|---|
| Name | shopsphere-bastion-01 |
| Role | Bastion Host |
| Environment | Production |
| Region | ap-south-1 |
| Subnet | shopsphere-public-subnet-1a |
| Security Group | shopsphere-bastion-sg |
| OS | Ubuntu Server |
| SSH | Restricted to administrator IP |

### Security Approach

SSH access is restricted to the administrator's public IP address.

The bastion host is located in a public subnet while application and database workloads will remain in private subnets.