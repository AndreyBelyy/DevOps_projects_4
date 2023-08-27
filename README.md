# DevOps_projects_4
Jenkins pipeline to run a Terraform script
Step 1:
Write the Terraform Code Create a new directory for your Terraform project. Inside the directory, create a main.tf file with the following Terraform code. (main.tf)
Step 2:
Install Required Plugins Ensure you have Jenkins installed, and then install the following plugins through the Jenkins Plugin Manager:
- AWS CLI Plugin
- Terraform Plugin
- Pipeline Utility Steps Plugin
Step 3:
Configure AWS Credentials To allow Jenkins to interact with AWS, you need to set up AWS credentials:
Go to “Manage Jenkins” > “Manage Credentials” > “Jenkins” Store.
Add a new “AWS Credentials” with your AWS Access Key ID and Secret Access Key.
