# SwarmServicesTerraform
Creating Docker Swarm Services Through Terraform

In this lesson, we will convert our Ghost and MySQL containers over to using Swarm services. Swarm services are a more production-ready way of running containers.

# Setup the environment:
**Linux Server - Installed with Docker-CE & Terraform

# Create a Folder.
mkdir -p SwarmServices
cd SwarmServices

**Initialize Terraform:
> terraform init

**Validate the files:
> terraform validate

**Build a plan:
> terraform plan -out=tfplan -var 'ext_port=8082'

**Apply the plan:
> terraform apply tfplan
> docker service ls
> docker container ls

**Destroy the environment:
> terraform destroy -auto-approve -var 'ext_port=8082'
