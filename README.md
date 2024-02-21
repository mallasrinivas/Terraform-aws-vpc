# Terraform VPC Deployment with Public and Private Subnets, Inter-Gateway, and Jenkins EC2 Instance

This Terraform project automates the deployment of a Virtual Private Cloud (VPC) infrastructure on AWS. The infrastructure includes public and private subnets, an Internet Gateway for outbound internet access, a NAT Gateway for private subnet internet access, and an EC2 instance with Jenkins installed in the public subnet.

## Prerequisites

- AWS account with appropriate permissions to create VPC, subnets, gateways, EC2 instances, and security groups.
- Terraform installed on your local machine.
- AWS CLI configured with appropriate access keys.

## Usage

1. Clone the repository to your local machine:
   ```bash
   git clone <repository-url>
   cd terraform-vpc-jenkins
   ```

````
2. Initialize Terraform:
```bash
terraform init
````

3. Review and customize the variables.tf file to match your environment requirements.

Review and customize the main.tf file to configure VPC settings, subnets, gateways, security groups, and EC2 instance settings.

Optionally, customize the userdata.sh script to include any additional setup steps for the Jenkins installation.

Plan the Terraform execution to review the changes:

```bash
terraform plan
```

4. Apply the Terraform execution to create the VPC infrastructure:

```bash
terraform apply
```

5. Review the output to obtain the public IP address of the Jenkins EC2 instance.
![image](https://github.com/mallasrinivas/Terraform-aws-vpc/assets/90713944/14939f1c-f64f-4381-b369-8e2cc6c18222)


