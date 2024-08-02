# Install Terraform and Visual Studio Terraform extension

To install Terraform in Visual Studio, follow these steps:

1. **Download Terraform**: Visit the official HashiCorp website and download Terraform based on your operating system [[3](https://medium.com/@mbbhawsar28/installation-of-terraform-and-visual-studio-code-fbf013d0db49)].

2. **Install Visual Studio Code**: If you haven't already, download and install Visual Studio Code on your machine [[4](https://k21academy.com/terraform-iac/install-visual-studio-code-for-terraform/)].

3. **Install Terraform Extension**: Open Visual Studio Code, go to the Extensions view by clicking on the square icon on the sidebar or pressing `Ctrl+Shift+X`. Search for the "Terraform" extension and install it. This extension provides syntax highlighting, linting, and other features for Terraform configuration files [[1](https://marketplace.visualstudio.com/items?itemName=HashiCorp.terraform)].

4. **Configure Terraform**: After installing the extension, configure the Terraform binary path in Visual Studio Code settings if it's not automatically detected. This ensures that Visual Studio Code can execute Terraform commands properly [[2](https://learn.microsoft.com/en-us/azure/developer/terraform/configure-vs-code-extension-for-terraform)].

5. **Verify Installation**: Once installed, verify that Terraform is correctly integrated into Visual Studio Code by creating or opening a Terraform project and accessing Terraform commands such as `terraform init`, `terraform plan`, and `terraform apply` from the integrated terminal.

Following these steps will enable you to use Terraform seamlessly within Visual Studio Code for managing your infrastructure as code.

## 🌐 Sources
1. [HashiCorp Terraform - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=HashiCorp.terraform)
2. [Install the Azure Terraform Visual Studio Code extension - Microsoft Docs](https://learn.microsoft.com/en-us/azure/developer/terraform/configure-vs-code-extension-for-terraform)
3. [Installation of Terraform and Visual Studio Code - Medium](https://medium.com/@mbbhawsar28/installation-of-terraform-and-visual-studio-code-fbf013d0db49)
4. [Install Visual Studio Code for Terraform and Plugins - k21academy.com](https://k21academy.com/terraform-iac/install-visual-studio-code-for-terraform/)

# Create a New GitHub Repository Named "Terraform"

1. **Log in to GitHub**: Open your web browser and navigate to [GitHub](https://github.com/). Log in to your GitHub account if you haven't already.

2. **Navigate to Repositories**: Once logged in, click on the "+" sign in the upper-right corner of the page, then select "New repository" from the dropdown menu.

3. **Fill in Repository Details**: 
   - Enter "Terraform" as the Repository name.
   - Optionally, add a description for your repository.
   - Choose whether the repository will be public or private.
   - If desired, initialize the repository with a README, .gitignore, or license.

4. **Create the Repository**: Click on the "Create repository" button. Your new GitHub repository named "Terraform" will be created.

5. **Clone the Repository (Optional)**: If you want to work with the repository locally on your computer, click on the green "Code" button and copy the repository URL. Open your terminal, navigate to the directory where you want to clone the repository, and run the command `git clone <repository_URL>`.

6. **Set Up Terraform Configuration (Optional)**: If you intend to manage infrastructure with Terraform, create your Terraform configuration files locally and commit them to the repository. This step is optional but recommended if you plan to use the repository for Terraform projects.

By following these steps, you'll have successfully created a new GitHub repository named "Terraform" and optionally set it up for use with Terraform projects.

## 🌐 Sources
1. [GitHub - Create a new repository](https://docs.github.com/en/github/getting-started-with-github/create-a-repo)
2. [How to Create GitHub Repository using Terraform - Medium](https://medium.com/@vijayalakshmiyvl/how-to-create-github-repository-using-terraform-cd2d4d204605)
3. [Example Terraform code to Create Github Repository - DevOpsSchool](https://www.devopsschool.com/blog/example-terraform-code-to-create-github-repository/)

# Clone the Terraform Repository in Visual Studio Code

1. **Open Visual Studio Code**: Launch Visual Studio Code on your computer.

2. **Open the Command Palette**: Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac) to open the Command Palette.

3. **Run Git Clone Command**: In the Command Palette, type "Git: Clone" and press Enter. Alternatively, you can press `Ctrl+Shift+G` (Windows/Linux) or `Cmd+Shift+G` (Mac).

4. **Enter Repository URL**: Paste the URL of the GitHub Terraform repository you want to clone into the input box and press Enter.

5. **Select Directory**: Choose the directory where you want to clone the repository. You can navigate to an existing directory or create a new one.

6. **Open Cloned Repository**: Once the cloning process is complete, Visual Studio Code will automatically open the cloned repository in a new window.

7. **Optional: Install Terraform Extension**: If you haven't already, you can install the Terraform extension for Visual Studio Code to enhance your Terraform development experience [[2](https://github.com/hashicorp/vscode-terraform)].

By following these steps, you'll successfully clone the GitHub Terraform repository in Visual Studio Code, allowing you to work with the Terraform files locally on your computer.

## 🌐 Sources
1. [HashiCorp Terraform VSCode extension](https://github.com/hashicorp/vscode-terraform)
2. [Working with Terraform – Git and Visual Studio Code - LinkedIn](https://www.linkedin.com/pulse/working-terraform-git-visual-studio-code-shubham-kumar-jain)
