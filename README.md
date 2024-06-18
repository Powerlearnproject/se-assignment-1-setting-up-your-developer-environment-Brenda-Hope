[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vbnbTt5m)

[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15290262&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11
   Check System Requirements:

Ensure your PC meets the minimum system requirements for Windows 11.
Download Windows 11:

Visit Microsoft's Windows 11 download page.
Click "Download now" to get the Windows 11 Installation Assistant.
Run Installation Assistant:

Open the downloaded file to run the Windows 11 Installation Assistant.
Follow Installation Steps:

The Assistant will guide you through upgrading or performing a fresh installation of Windows 11.
Follow on-screen prompts to proceed with installation.
Setup and Personalize:

Configure user accounts, privacy settings, and other preferences during setup.
Install Drivers and Updates:

After installation, install necessary drivers and check for Windows updates.
Install Software:

Install applications like Visual Studio Code, Git, and other tools as needed.
Backup and Precautions:

Backup important data before proceeding with installation.

3. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download
   Go to Visual Studio Code Download.
Select Your Operating System:

Choose Windows, macOS, or Linux, and download the installer.
Run the Installer:

Open the downloaded file and follow the installation prompts.
Open Visual Studio Code:

Launch VS Code after installation completes.
Install Extensions (Optional):

Customize VS Code by installing extensions (Ctrl+Shift+X or Cmd+Shift+X).
Configure Settings (Optional):

Adjust settings through File > Preferences (Windows/Linux) or Code > Preferences (macOS).
Start Coding.
4. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com
   Download Git from https://git-scm.com/ and follow installation instructions for your operating system.
Configure Git:

Set up your username and email in Git using the  commands
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
Create a GitHub Account and sign up
Initialize a Git Repository:

Navigate to your project folder in the terminal or command prompt.
Initialize a new Git repository
  git init
Add and Commit Files
  git add .
  git commit -m "Initial commit"
Create a Repository on GitHub:

Log in to GitHub and create a new repository.
Follow the instructions to add a remote repository (the URL provided after creating a repository on GitHub)
  git remote add origin <repository_URL>
Push Changes to GitHub:
Push your committed changes to GitHub
  git push -u origin master

5. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.
Go to python.org in your web browser.
Click on the "Downloads" tab.
Choose Python Version:

Python releases are available in two major versions: Python 2.x and Python 3.x. It's recommended to use Python 3.x (where x is the latest version available).
Select the version suitable for your project. As of my last update, Python 3.10 or newer versions are commonly available.
Download Installer:

Click on the download link for the installer corresponding to your operating system (Windows, macOS, or Linux).
Run Installer:

Once downloaded, run the installer executable.
On Windows: Check the box that says "Add Python to PATH" during the installation process. This makes it easier to run Python from the command line.

Verify Installation:

Open a command prompt or terminal.
Type python --version or python3 --version (depending on your system and Python version).
You should see the installed Python version printed out.
Installing Compilers, Interpreters, or Runtimes


Windows: You can install GCC through MinGW or use Visual Studio.
macOS: Install Xcode Command Line Tools which include Clang.
Linux: Install GCC through your package manager (e.g., sudo apt install build-essential on Ubuntu).
For Java: Install JDK (Java Development Kit).

Download JDK from Oracle's website and follow the installation instructions.
For .NET Framework: Install .NET SDK.

Download from .NET SDK downloads and follow the installation instructions.
For JavaScript/Node.js: Install Node.js.

Download from Node.js official website and follow the installation instructions.
Setting Up Your Development Environment
Integrated Development Environment (IDE):

Choose an IDE such as PyCharm, Visual Studio Code, or any other preferred IDE that supports Python and your project's languages.
Package Management:

Use pip (Python's package installer) to manage Python packages. It comes installed by default with Python 3.4 and above.
Virtual Environments:

Consider using virtual environments (virtualenv or venv) to manage dependencies and isolate your project's environment.

7. Install Package Managers:
   If applicable, install package managers like pip (Python).
    To install `pip`, which is the package manager for Python, you typically don't need to do anything extra if you've installed Python using the official installer from [python.org](https://www.python.org/). Here’s how you can verify and use `pip`:

### Verify pip Installation


9. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html
   Visit the MySQL Download Page:
Go to the MySQL official website to download the MySQL Community Server: MySQL Downloads

Select the MySQL Edition:

Choose the MySQL Community Server edition suitable for your operating system (Windows, macOS, Linux, etc.).
Ensure to download the version compatible with your OS and requirements.
Download MySQL Installer:

Click on the download button for the MySQL Installer appropriate for your operating system.
The installer usually includes MySQL Server and other tools like MySQL Workbench for database management.
Install MySQL
Windows Installation Steps:
Run the Installer:

Once downloaded, run the MySQL Installer executable (.exe file).
Choose Setup Type:

Select the setup type. For most users, the "Developer Default" is suitable, as it includes MySQL Server and additional tools.
Installation Process:

Follow the installation wizard instructions.
Specify the installation directory and configure MySQL Server settings as needed (like port number, server instance configuration, etc.).
Configure MySQL Server:

During installation, you will be prompted to set a root password for MySQL. Choose a strong password and remember it for future use.
Complete Installation:


Optionally, you can choose to launch MySQL Workbench or any other tools included in the installer.

11. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.
Install Docker:

Windows/macOS: Download and install Docker Desktop from Docker's official website.
Linux: Follow Docker’s installation guide for your specific distribution.
2. Create a Dockerfile:

A Dockerfile is a text document that contains all the commands needed to assemble an image. Here’s a basic example for a MySQL database setup
   # Use an official MySQL runtime as a parent image
FROM mysql:latest

# Set the root password
ENV MYSQL_ROOT_PASSWORD=password

# Specify the database to be created when the container starts
ENV MYSQL_DATABASE=mydatabase

# Optionally, specify the MySQL port
EXPOSE 3306
Build and Run the Docker Container:

Navigate to the directory where your Dockerfile is located.
Build the Docker image
 docker build -t my-mysql-image .
Run the Docker container based on the image
 docker run -d --name my-mysql-container -p 3306:3306 my-mysql-image
 -d flag runs the container in detached mode.
--name specifies a name for the container.
-p maps port 3306 from the container to port 3306 on the host (adjust as needed).
4. Connect and Use MySQL:

Use MySQL client tools to connect to the MySQL instance running inside the Docker container. For example
 mysql -h localhost -P 3306 -u root -p
Enter the password specified in the Dockerfile 
12. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.
   Linting: Checks your code for errors, potential bugs, or stylistic issues, providing real-time feedback as you write code.

Code Formatting: Automatically formats your code according to predefined rules or style guides, ensuring consistency and readability.

Version Control Integration: Enables seamless integration with version control systems like Git, allowing you to commit, pull, push, and manage branches directly from your IDE.

Debugging Tools: Provides tools for debugging code, setting breakpoints, inspecting variables, and stepping through code execution


13. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process.
    9. Operating System
Operating System: Windows 10 Pro
Version: 21H2
Development Tools
Integrated Development Environment (IDE):

IDE: Visual Studio Code (VS Code)
Extensions Installed:
Python (ms-python.python)
GitLens (eamodio.gitlens)
Docker (ms-azuretools.vscode-docker)
ESLint (dbaeumer.vscode-eslint)
Live Server (ritwickdey.liveserver)
Version Control:

Version Control System: Git
Git Client: Git Bash
Programming Languages:

Python:
Version: 3.9.7
Installed using Anaconda distribution
Containerization:

Docker:
Installed Docker Desktop for Windows
Configured Docker settings and allocated necessary resources
Configurations and Customizations
Visual Studio Code:

Settings Customizations:
Configured Python interpreter path to use Anaconda Python distribution.
Modified font size, theme (Dark+), and indentation settings.
Git Configuration:

Global Configurations:
Set username and email for Git commits.
Configured default branch name to main.
Troubleshooting
Issue: Docker containers failing to start.

Resolution: Increased Docker resources (CPU, Memory) allocation in Docker Desktop settings.
Issue: Python extension in VS Code not recognizing interpreter.

Resolution: Manually set the Python interpreter path in VS Code settings to point to Anaconda Python installation.

#Deliverables:
- Document detailing the setup process with step-by-step instructions and screenshots where necessary.
- A GitHub repository containing a sample project initialized with Git and any necessary configuration files (e.g., .gitignore).
- A reflection on the challenges faced during setup and strategies employed to overcome them.

#Submission:
Submit your document and GitHub repository link through the designated platform or email to the instructor by the specified deadline.

#Evaluation Criteria:**
- Completeness and accuracy of setup documentation.
- Effectiveness of version control implementation.
- Appropriateness of tools selected for the project requirements.
- Clarity of reflection on challenges and solutions encountered.
- Adherence to submission guidelines and deadlines.

Note: Feel free to reach out for clarification or assistance with any aspect of the assignment.
