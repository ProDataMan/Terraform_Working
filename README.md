# Clone the Terraform_Working repo
git clone https://github.com/ProDataMan/Terraform_Working.git

# Copy terraform.exe.sav to c:\software\terraform.exe (for windows)
drag and drop

Note: If you are running Mac download the Mac version of Terraform

# Terraformn Download
https://developer.hashicorp.com/terraform/install

# Create an Access Key in AWS
search for the IAM service in the AWS Console
Select users in the menu on the left under Access Management
Find your user name in the list and click on it
Click on Create Access Key (upper right)
Select Applications running outside of AWS
Click Next
Add a description to your key (Deployment Key)
Click Create Access Key

# Install AWS CLI
Windows
https://awscli.amazonaws.com/AWSCLIV2.msi

Mac
https://awscli.amazonaws.com/AWSCLIV2.pkg

# configure AWS
aws configure

Enter you AWS Access Key ID
Enter you AWS Secret Access Key
Enter us-west-1 as the Default region name
Accept the Default output format [None] (press enter)

# Initialize Terraform
c:\software\terraform init
