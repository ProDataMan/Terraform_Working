# Clone the Terraform_Working repo
git clone https://github.com/ProDataMan/Terraform_Working.git

# Copy terraform.exe.sav to c:\software\terraform.exe (for windows)
drag and drop

Note: If you are running Mac download the Mac version of Terraform

# Terraformn Download
https://developer.hashicorp.com/terraform/install

# Create new IAM User and add permissions policy
Step 1: Sign in to the AWS Management Console
Go to the AWS Management Console and sign in with your AWS credentials.
Step 2: Navigate to the IAM Console
In the AWS Management Console, go to Services and select IAM (Identity and Access Management) from the Security, Identity, & Compliance section.
Step 3: Create a New IAM User
In the IAM dashboard, click on Users in the left-hand navigation pane.
Click on the Add user button.
Step 4: Configure User Details
Enter a User name (e.g., terraform-user).
Under Select AWS access type, check Programmatic access.
Click Next: Permissions.
Step 5: Set Permissions
Choose Attach existing policies directly.
Click on the Create policy button to open a new tab for policy creation.
Step 6: Create the Policy
In the new tab for the Create policy page, switch to the JSON tab.

Copy and paste the example policy JSON below into the editor:

json
Copy code
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "ec2:*",
        "s3:*",
        "rds:*",
        "iam:*",
        "sts:GetCallerIdentity",
        "cloudwatch:*",
        "logs:*",
        "autoscaling:*",
        "elasticloadbalancing:*"
      ],
      "Resource": "*"
    }
  ]
}
Click on the Review policy button.

Enter a Name for the policy (e.g., TerraformPolicy).

(Optional) Enter a Description.

Click Create policy.

Step 7: Attach the Policy to the New User
Go back to the tab where you are creating the new user.
Refresh the policy list by clicking the refresh icon next to the search box.
Search for the policy you just created (e.g., TerraformPolicy).
Check the box next to the policy to attach it to the user.
Click Next: Tags.
Step 8: Add Tags (Optional)
Add any tags you need for your user. Tags are key-value pairs that can help you organize and manage your AWS resources.
Click Next: Review.
Step 9: Review and Create the User
Review the user details and the attached policy.
Click Create user.
Step 10: Download Credentials
On the confirmation page, click Download .csv to save the user's access key ID and secret access key. You will need these credentials to configure Terraform.
Click Close.
Configuring AWS CLI with the New User’s Credentials
Open your terminal or command prompt.

Run the following command to configure the AWS CLI:

bash
Copy code
aws configure
Enter the Access Key ID and Secret Access Key from the .csv file you downloaded:

plaintext
Copy code
AWS Access Key ID [None]: YOUR_ACCESS_KEY_ID
AWS Secret Access Key [None]: YOUR_SECRET_ACCESS_KEY
Default region name [None]: us-west-2
Default output format [None]: json

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
