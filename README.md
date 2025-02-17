# aws-terraform-webserver
Made for Relx Practice Assessment


# AWS EC2 Terraform Web Server

## Prerequisites
- AWS Account
- Terraform installed
- AWS CLI configured

## Steps to Deploy
1. Clone this repository:
   ```sh
   git clone https://github.com/YOUR_GITHUB_USERNAME/aws-terraform-webserver.git
   cd aws-terraform-webserver
Initialize and apply Terraform:

  terraform init
  terraform apply -auto-approve

Get the public IP and access the web server:

  terraform output instance_public_ip
  Open http://<PUBLIC_IP> in a browser.

Monitoring
  
CloudWatch tracks CPU usage.

CI/CD Pipeline

GitHub Actions validates Terraform on every push.

Cleanup
To destroy resources:

terraform destroy -auto-approve


---

## **Step 8: Cleanup**
To remove all resources:
```sh
terraform destroy -auto-approve
