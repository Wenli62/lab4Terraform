# lab4Terraform
- Instructions on general set up.
1. create a directory and run `terraform init` first
3. create key pair with ssh-keygen command, import public key into AWS EC2 key pair
4. configure cloud-config.yaml to let it handle ssh session and packages installation in the EC2 instance
5. configure .tf file to plan necessary resource for infrastructure
6. run `terraform validate`, `terraform plan`, `terraform apply` in this specific order to provision the resources
7. run `terraform destroy` to delete all provisioned resources

- Command used to create a new SSH key pair.
ssh-keygen -t ed25519 -f ~/lab4key
- Commands used to initialize, fmt, plan... configuration.
initialization: `terraform init`
format the configuration file: `terraform fmt`
validate syntax in configuration: `terraform validate`
review resouces before provisioning: `terraform plan`
configuration: `vim *.tf`
- Any other instructions needed to setup configuration
