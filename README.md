# azurepilot

## Station Setup
* VS Code: format on save, terraform extension
* Chocolately: https://chocolatey.org/install
* Terraform: terraform.io or __choco install terraform -y__
* Python and Azure CLI or __choco install azure-cli -y__
* Git bash or __choco install git -y__

NOTE: chocolatey installs **terraform.exe** in C:\ProgramData\chocolatey\lib\terraform\tools

set repo & open in VS code
main.tf
terraform init
terraform plan
terraform apply
terraform destroy


## Goals
* TF templates for HA Web Server with VM, LB, Autoscaler, IIS
* PowerShell and CLI scripts
* KQL security queries
* Data Factory deployment and pipelines
