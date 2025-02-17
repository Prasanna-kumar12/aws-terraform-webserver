# aws-terraform-webserver
Made for Relx Practice Assessment


# AWS EC2 Terraform Web Server

## Prerequisites
- AWS Account
- Terraform installed
- AWS CLI configured

 **Authenticate AWS CLI**
   Run the following command and enter your AWS credentials:
   
    aws configure
    
 You'll need to enter:
  AWS Access Key
  AWS Secret Key
  Default AWS Region (e.g., us-east-1)
  Output Format (choose json)

## Steps to Deploy
1. Clone this repository:
   ```sh
   git clone https://github.com/YOUR_GITHUB_USERNAME/aws-terraform-webserver.git
   cd aws-terraform-webserver
   
2.Initialize and apply Terraform:

    terraform init
    terraform apply -auto-approve

3.Get the public IP and access the web server:

    terraform output instance_public_ip
   Open http://<PUBLIC_IP> in a browser.

4.Monitoring
   CloudWatch tracks CPU usage.

5.CI/CD Pipeline

  GitHub Actions validates Terraform on every push.

    git add .
    git commit -m "Initial Terraform setup"
    git push origin main
 
6.Cleanup
    To destroy resources:

     terraform destroy -auto-approve

## **Step 8: Cleanup**
To remove all resources:
```sh
terraform destroy -auto-approve
