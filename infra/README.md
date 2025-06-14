# Terraform Github Actions 

### Infra directory

    main.tf - Primary file implementing all the terraform code
    output.tf - Stores all output definitions
    providers.tf - Stores all provider configurations
    terraform.auto.tfvars - Stores values of all variable definitions
    variables.tf - Stores all variable definitions.

### Create a key pair from the cli:

#### example: 

aws ec2 create-key-pair --key-name "terraform-gha" --region us-east-1 --query 'KeyMaterial' --output text > terraform-gha.pem
