# Terraform Docker Container Provisioning

**Author:** Mithula

**GitHub Repository:** https://github.com/Mithula7777/terraform-docker-project

## Project Overview

This project demonstrates how to provision a Docker container using Terraform. Terraform is used as an Infrastructure as Code (IaC) tool to manage Docker resources.

The project uses the Docker provider to download the Nginx image and create a running Docker container.

## Tools and Technologies

- AWS EC2 – Amazon Linux
- Terraform
- Docker
- Nginx

## Project Objective

To automate the creation and management of a Docker container using Terraform.

## Project Implementation

1. Installed Docker on the Amazon Linux EC2 instance.
2. Installed Terraform.
3. Configured the Terraform Docker provider.
4. Created the `main.tf` configuration file.
5. Downloaded the Nginx Docker image using Terraform.
6. Created a Docker container named `terraform-nginx`.
7. Mapped container port 80 to host port 8080.
8. Verified the Nginx welcome page using `curl`.
9. Checked resources using Terraform state commands.
10. Destroyed the resources using Terraform.

## Terraform Commands

```bash
terraform init
terraform validate
terraform plan
terraform apply
terraform state list
terraform state show docker_container.nginx
terraform destroy
```

## Verification

The Nginx application was verified using:

```bash
curl http://localhost:8080
```

The Nginx welcome page was displayed successfully.

## Project Files

- `main.tf` – Terraform configuration file.
- `execution-logs.txt` – Terraform execution logs.

## Cleanup

The resources were removed successfully using:

```bash
terraform destroy
```

## Result

Successfully provisioned and verified an Nginx Docker container using Terraform on an AWS EC2 Amazon Linux instance.

**Project Status: Completed**

**Author: Mithula**
