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

## Git Repo
NOTE: .gitignore should include *.bak and *~ 

* mkdir ./tfcaf && cd ./tfcaf
* touch README.md (can add notes via nano)
* git init --initial-branch=main (older version __git checkout -b main__)
* git status (which changes are currently being tracked)
* git add . (all files in current dir) OR git add -A (add any _untracked_ files)
* git commit -m "add notes"
* git remote add origin https://github.com/usr/repo (git@github.com:<username>/<repository>.git)
* git push origin main

**Branch Create & Merge**
PREBRANCH CHECKPOINT
* git switch master
* git commit -m "PREMERGE SAFETY COMMIT & DIFF"

CREATE BRANCH
* git checkout -b MyNewBranch (create and switch to mybranch)
* git push origin MyNewBranch  
* git branch (show branch)
* git add .
* git commit -m "updates to MyNewBranch"

PULL REQUEST
* git push -u origin MyNewBranch
* navigate GitHub site to approve pull requests
https://github.com/<usr>/<repo>/pull/new/branch


MERGE BRANCH
* git diff MyNewBranch (use 'q' to exit)
* git status
* git checkout main (check out the target / destination branch)
* git merge MyNewBranch

OPTIONS FOR CONFLICT RESOLUTION
git merge master --strategy==theirs
#make THEIR changes win

git merge master --strategy=ours
#make OUR changes win

UNDO STAGED CHANGES
* git reset <filename> (ex README.md)
* git status (verify)

UNDO COMMITS
* git reset HEAD~1 (one commit back from HEAD)
* git status
* git diff





## Terraform Template

* versions.tf
* variables.tf
* main.tf
* outputs.tf
* terraform.tfvars


