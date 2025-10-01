🚀 Terraform AWS EC2 Demo
This project provisions an Amazon EC2 instance on AWS using Terraform to demonstrate Infrastructure as Code (IaC). It highlights the basic Terraform workflow and shows how infrastructure can be deployed in a consistent, repeatable, and version-controlled way.
🛠 Tech Stack
Terraform
AWS (EC2, IAM)
GitHub Actions (optional for CI/CD integration)
📂 Project Structure
terraform-aws-ec2-demo/
├── main.tf         # EC2 resource definition
├── provider.tf     # AWS provider configuration
├── variables.tf    # Input variables (instance type, region, etc.)
├── outputs.tf      # Outputs (e.g. public IP, instance ID)
├── terraform.tfvars # Variable values (not committed if sensitive)
⚙️ How It Works
Define infrastructure in Terraform files (.tf).
Initialize Terraform to download provider plugins.
Plan the changes to preview what will be deployed.
Apply to provision the EC2 instance.
Destroy when you no longer need the resources.
🚦 Usage
Clone the repo and navigate into it:
git clone https://github.com/777-888/terraform-aws-ec2-demo.git
cd terraform-aws-ec2-demo
Initialize Terraform:
terraform init
Preview the changes:
terraform plan
Deploy the EC2 instance:
terraform apply
Destroy resources when finished:
terraform destroy
🔑 Variables
Variable	Description	Default
region	AWS region to deploy into	eu-west-2
instance_type	EC2 instance type	t2.micro
ami_id	Amazon Linux 2 AMI ID (region-specific)	None
📤 Outputs
EC2 Public IP
Instance ID
Example output after terraform apply:
