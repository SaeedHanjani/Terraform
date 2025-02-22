# Terraform
Best practice for Terraform
Terraform is an infrastructure-as-code software tool created by HashiCorp. Users define and provide data center infrastructure using a declarative configuration language known as HashiCorp Configuration Language, or optionally JSON.
# What is Terraform?
Terraform is an infrastructure as code tool that lets you build, change, and version infrastructure safely and efficiently. This includes low-level components like compute instances, storage, and networking; and high-level components like DNS entries and SaaS features.

### IaC or Infrastructure as Code 
# why we need IaC
1. Decreased risk
2. Stable & consistent environments for faster iterations
3. Cost optimization
4. Self-documenting

IaC Tools
1. Terraform
2. AWS Cloud Formation: using a Yaml File
3. Azure Resource Manager
4. Google Cloud Deployment Manager
5. Pulumi
6. CDKTF
7. Ansible
8. Puppet

ما می توانیم از AWS بصورت مستقیم یک فایل yaml بسازیم و سپس باهاش ساختارمون رو بیاریم بالا، ولی این روی Asure یا ابزارهای دیگه کار نمیکند.
راه حل: ترافورم گفت بیا از ابزار من استفاده کن و پشت قضیه رو به هر چیزی که میخوای مثل آمازون یا ماکروسافت وصل کن.

# Configuration management vs Infrastructure Orchestration
Terraform and cloudformation are tools to configure the cloud But ansible and puppet are Configuration management tools and their main purpose is to do some configuration on the target OS.

# Terraform Providers and basic AWS configuration to get programmatic acces
# Confiure mian.tf for AWS
first you create a an acount for aws and after that you config budget . so you need a user with limited access. after that you create key access (public and secrec key).
we create repo on github and pull on my mac. after that create  main.tf and copy data for initialize. we write terraform init in cmd of mac.
if your terraform is not update, you see warning for need to updating your terraform.

# create your first resource with terraform

##Workflow Summary (Your ESXi VM Creation)

##    terraform init:
        Sets up the vsphere provider so Terraform can talk to ESXi.
##    terraform validate:
        Confirms your main.tf is syntactically correct and logical.
##    terraform plan:
        Previews that Terraform will create a VM with your specified settings.
##    terraform apply:
        Connects to ESXi and builds the VM.
