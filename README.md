A Terraform module to provision an AWS EC2 instance with the latest Amazon Linux 2023 AMI and Docker installed on it.

Not intended for production use. It serves as an example module.

This is just to demonstrate how to create and publish a module on the Terraform Registry.

Usage:

```hcl

provider "aws" {
  region = "us-east-1"
}

module "docker_instance" {
    source = "engin-nvr/instance-for-docker-use/aws"
    key_name = "clarusway"
}
```
