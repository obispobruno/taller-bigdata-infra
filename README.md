# Azure Big Data Infrastructure

This Terraform configuration sets up the basic networking infrastructure for a big data environment in Azure, including:

- A virtual network with a subnet
- A network security group with SSH access

## Prerequisites

- [Terraform](https://www.terraform.io/downloads.html) installed (version 1.0.0 or later)
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli) installed
- An Azure subscription
- Azure CLI authenticated with your Azure account

## Configuration

The configuration creates:

- A resource group in East US region
- A virtual network with address space 10.0.0.0/24
- A subnet using the entire address space
- A network security group allowing SSH access (port 22)

## Usage

1. If not already logged in, login to azure:

```bash
az login
```

2. Initialize Terraform:

```bash
terraform init
```

3. Review the planned changes:

```bash
terraform plan
```

4. Apply the configuration:

```bash
terraform apply
```

5. To destroy the infrastructure when no longer needed:

```bash
terraform destroy
```
