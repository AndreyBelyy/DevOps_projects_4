# DevOps_projects_4
Jenkins pipeline to run a Terraform script
- Step 1:
Write the Terraform Code Create a new directory for your Terraform project. Inside the directory, create a main.tf file with the following Terraform code. (main.tf)
 - Step 2:
Install Required Plugins Ensure you have Jenkins installed, and then install the following plugins through the Jenkins Plugin Manager:
  1. AWS CLI Plugin
  2. Terraform Plugin
  3. Pipeline Utility Steps Plugin
 - Step 3:
Configure AWS Credentials To allow Jenkins to interact with AWS, you need to set up AWS credentials:
Create a new user in IAM in AWS or use the existing one.
Go to “Manage Jenkins” > “Manage Credentials” > “Jenkins” Store.
Add a new “AWS Credentials” with your AWS Access Key ID and Secret Access Key.
 - Step 5:
Set up your Terraform Code Repository Create a Git repository with your Terraform code, including the main.tf file that describes your desired EC2 instance.
Write the Jenkinsfile In your Terraform code repository, create a Jenkinsfile (Jenkinsfile)
 - Step 6:
Configure Jenkins Job
      a) In Jenkins, create a new pipeline job
      b) Under the “Pipeline” section, select “Pipeline script from SCM.”
      c) Provide the repository URL and specify the Jenkinsfile location (e.g., Jenkinsfile)
      d) Save the job configuration
 - Step 7:
Run the Jenkins Job Now, you can run the pipeline job to execute your Terraform code and provision an EC2 instance. Jenkins will fetch the code from the repository, initialize Terraform, create a plan, apply the changes, and upload the Terraform state to an S3 bucket.
 - Credits to Praveen Dandu (https://praveendandu24.medium.com/how-to-run-a-terraform-script-in-jenkins-a-step-by-step-guide-21edb0cbe6b2)
