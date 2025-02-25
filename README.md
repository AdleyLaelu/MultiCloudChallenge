☁️ MultiCloud, DevOps & AI Challenge - Day 1 - Automating AWS provisioning using Terraform ☁️
This is part of the first project of the challenge/bootcamp!

In this project we will be setting up our whole set of project for this challenge utilizing terraform to create a S3 bucket and create a DynamoDB table which will be the basis and start of our project.

Environments and Technologies Used
Terraform
Amazon Web Services
Github Codespaces
S3
DynamoDB
Features
In here we learn how to deploy AWS services using Terraform in a automated and efficient way.
Step by Step Instructions
1. Repo configuration

NOTE: Keep in mind this is for a Linux environment, check the AWS documentation to install it in your supported OS.

curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" unzip awscliv2.zip sudo ./aws/install

We then do AWS configure and enter our access and secret key along with the region. Output format set to JSON. With this command we will double check that our credentials are put in place for CLI:

aws sts get-caller-identity
We will then install terraform CLI:

sudo wget -O - https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform
2. Terraform Configuration

In this step we will make sure that we have terraform set up.

First, we will create a terraform folder and point to it directly:

mkdir terraform-project && cd terraform-project
Then we will initialize the terraform plaform with the main.tf file. Inside it, is the documentation to create a S3 bucket

terraform init
Next, we will review the plan:

terraform plan
Finally, we will apply it.

terraform apply
We will verify our bucket and dynamoDB table was created successfully with the AWS CLI command:

aws s3 ls

3. Final Result

This will be the S3 bucket and DynamoDB table created with Terraform, as shown in the console:
