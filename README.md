[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15248147&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11

   WHAT DO YOU NEED.
1.	Windows installation media. This could be an installation ISO or DVD.
2.	USB flash drive with at least 5GB free space,ensure the flash disk has nothing important since it will be formatted.
3.	Technician PC - Windows PC that you'll use to format the USB flash drive
4.	Destination PC - A PC that you'll install Windows on

Step 1 - Format the drive and set the primary partition as active.
1.	Connect the USB flash drive to your technician PC.
2.	Open Disk Management: Right-click on Start and choose Disk Management.
3.	Format the partition: Right-click the USB drive partition and choose Format. Select the FAT32 file system to be able to boot either BIOS-based or UEFI-based PCs.
4.	Set the partition as active: Right-click the USB drive partition and click Mark Partition as Active.

Step 2 - Copy Windows Setup to the USB flash drive.
1.	Use File Explorer to copy and paste the entire contents of the Windows product DVD or ISO to the USB flash drive.
2.	Optional: add an unattend file to automate the installation process. For more information, see Automate Windows Setup.


Step 3 - Install Windows to the new PC.
•	Connect the USB flash drive to a new PC.
•	Turn on the PC and press the key that opens the boot-device selection menu for the computer, such as the Esc/F10/F12 keys. Select the option that boots the PC from the USB flash drive.
•	Windows Setup starts. Follow the instructions to install Windows.
•	Remove the USB flash drive.
https://1drv.ms/w/c/f8222d6573680bb4/Ebe2NhOv7xVGqxKSmUGpZvYB-e6ApqdFVWRiai3bFMZyGw
            


2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download
   1.	Download the VS Code file 
   2.	Execute the download file.
   3.	Accept the Terms & Conditions.
   4.	Click on the Install button.
   5.	Wait for the installation to complete.
   6.	Click on the Launch button to start it.
   https://1drv.ms/w/c/f8222d6573680bb4/EfOzv42RpOhOnNfh2MaYd_IBE1WNowEP0xlinSyXUiiSsg?e=WsVZej

3. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com
   Step 1: Install Git
1. For Windows:
   - Download Git from [git-scm.com](https://git-scm.com/).
   - Run the installer and follow the instructions. Use the default settings unless you have a specific reason to change them.
   - Open Git Bash from the start menu after installation is complete.

Step 2: Configure Git
1. Open your terminal or Git Bash.
2. Set your username:
   ```bash
   git config --global user.name "Your Name"
   ```
3. Set your email:
   ```bash
   git config --global user.email "your.email@example.com"
   ```

 Step 3: Create a GitHub Account
1. Go to [GitHub](https://github.com/).
2. Sign up for a new account if you don't already have one.

Step 4: Initialize a Git Repository
1. Create a new directory for your project:
   ```bash
   mkdir my-project
   cd my-project
   ```
2. Initialize a new Git repository:
   ```bash
   git init
   ```

Step 5: Create a New File and Make Your First Commit
1. Create a new file in your project directory. For example, create a `README.md` file:
   ```bash
   echo "# My Project" > README.md
   ```
2. Add the file to the staging area:
   ```bash
   git add README.md
   ```
3. Commit the file:
   ```bash
   git commit -m "Initial commit"
   ```

Step 6: Push to GitHub
1. Create a new repository on GitHub:
   - Go to your GitHub account.
   - Click on the "New" button to create a new repository.
   - Enter the repository name (e.g., `my-project`), and click "Create repository".

2. Link your local repository to the GitHub repository:
   ```bash
   git remote add origin https://github.com/your-username/my-project.git
   ```

3. Push your commits to GitHub:
   ```bash
   git push -u origin master
   ```



4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.
  Step 1: Install Python

1. Download Python:
   - Download the latest version of Python for your operating system.

2. Install Python:
   - Run the installer.
   - Make sure to check the box that says "Add Python to PATH".
   - Follow the installation instructions.

Step 2: Verify the Installation

1. Open a terminal (Command Prompt, PowerShell, or Git Bash).
2. Check the Python version:
   ```bash
   python --version
   ```
   or
   ```bash
   python3 --version
   ```

Step 3: Install pip (Python Package Installer)

`pip` is usually included with Python installation. Verify its installation by running:
```bash
pip --version
```
If `pip` is not installed, you can install it manually:
1. Download `get-pip.py`:
   - Go to https://bootstrap.pypa.io/get-pip.py.
   - Save the file as `get-pip.py`.

2. Run `get-pip.py` using Python:
   ```bash
   python get-pip.py
   ```

Step 4: Install Necessary Packages

Depending on your project, you might need additional Python packages. Use `pip` to install them. For example:
```bash
pip install numpy pandas matplotlib
```
Replace `numpy pandas matplotlib` with the packages you need for your project.

### Step 5: Verify Installation of Packages

To verify that the packages are installed correctly, you can try importing them in Python:
1. Open a Python interpreter:
   ```bash
   python
   ```
2. Try importing the installed packages:
   ```python
   import numpy
   import pandas
   import matplotlib
   ```
If there are no errors, the packages are installed correctly.

Step 6: Set Up a Virtual Environment 

Using a virtual environment is a good practice to manage dependencies for your project.

1. Install `virtualenv` using `pip`:
   ```bash
   pip install virtualenv
   ```

2. Create a virtual environment:
   ```bash
   virtualenv venv
   ```
3. Activate the virtual environment:
   - On Windows:
     ```bash
     .\venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```
4. Deactivate the virtual environment when done:
 ```bash
   deactivate


5. Install Package Managers:
   If applicable, install package managers like pip (Python).
   The process of installing package managers like `pip` for Python.

 Step 1: Ensure pip is Installed


Verify pip Installation

1. Open a terminal (Command Prompt, PowerShell, or Git Bash).
2. Check the pip version:
   ```bash
   pip --version
   ```

If `pip` is installed, you will see output showing the version of `pip` installed.

Install pip (if not already installed)

If `pip` is not installed, you can install it manually:

1. Download `get-pip.py`:
   - Go to https://bootstrap.pypa.io/get-pip.py.
   - Save the file as `get-pip.py`.

2. Run `get-pip.py` using Python:
   ```bash
   python get-pip.py
   ```

 Step 2: Install and Verify Common Package Managers for Different Languages

Here are the steps for some other popular package managers:

#### Node.js and npm (JavaScript/Node.js)

1. Download Node.js from the official website:
   - Go to https://nodejs.org/.
   - Download and install the LTS version, which includes `npm`.

2. Verify npm installation:
   ```bash
   npm --version
   ```

Ruby and Bundler (Ruby)

1. Install Ruby:
   - Download Ruby from https://www.ruby-lang.org/en/downloads/.
   - Follow the installation instructions for your operating system.

2. Install Bundler:
   ```bash
   gem install bundler
   ```

3. Verify Bundler installation:
   ```bash
   bundler --version
   ```

Homebrew (macOS)

1. Install Homebrew:
   - Open Terminal and run:
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```

2. Verify Homebrew installation:
   ```bash
   brew --version
   ```

Composer (PHP)

1. Download Composer:
   - Go to https://getcomposer.org/download/.
   - Follow the installation instructions for your operating system.

2. Verify Composer installation:
   ```bash
   composer --version
   ```


1. Python (pip):
   - `pip` is usually installed with Python. Verify with:
     ```bash
     pip --version
     ```
   - If not installed, use:
     ```bash
     python get-pip.py
     ```

2. JavaScript (npm):
   - Install Node.js which includes `npm` from https://nodejs.org/.
   - Verify with:
     ```bash
     npm --version
     ```

3. Ruby (Bundler):
   - Install Ruby from https://www.ruby-lang.org/en/downloads/.
   - Install Bundler with:
     ```bash
     gem install bundler
     ```
   - Verify with:
     ```bash
     bundler --version
     ```

4. macOS (Homebrew):
   - Install Homebrew with:
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```
   - Verify with:
     ```bash
     brew --version
     ```

5. PHP (Composer):
   - Install Composer from https://getcomposer.org/download/.
   - Verify with:
     ```bash
     composer --version
     ```





6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html
    Steps to download, install, and configure a MySQL database on a Windows machine.

Step 1: Download MySQL Installer

1. Go to the MySQL Download Page:
   - Open your web browser and go to [MySQL Downloads](https://dev.mysql.com/downloads/windows/installer/5.7.html).

2. Download the MySQL Installer:
   - Click on the "Download" button for the MySQL Installer.
   - Choose either the "Web Community" (smaller file) or the "Full" (larger file) installer. The web installer will download the necessary components during the installation process.

Step 2: Install MySQL

1. Run the Installer:
   - Once the download is complete, run the installer.

2. Choose Setup Type:
   - In the setup window, you will see different setup types (Developer Default, Server only, etc.). Choose "Custom" if you want to select specific components or "Developer Default" for a full installation suitable for most users.

3. Select Products and Features:
   - In the "Select Products and Features" screen, make sure the MySQL Server, MySQL Workbench, and other necessary tools are selected.

4. Check Requirements:
   - The installer will check for any missing requirements. Install any additional required software as prompted.

5. Installation:
   - Proceed with the installation by clicking "Execute" to download and install the selected products.

 Step 3: Configure MySQL Server

1. Product Configuration:
   - After the installation, the MySQL installer will prompt you to configure the server. Click "Next" to begin configuration.

2. Configuration Type:
   - Choose the configuration type that best suits your needs. "Development Machine" is usually sufficient for development purposes.

3. Connectivity:
   - Leave the default port (3306) and click "Next".

4. Authentication Method:
   - Choose the authentication method. The recommended option is "Use Strong Password Encryption for Authentication (RECOMMENDED)".

5.Accounts and Roles:
   - Set the root password for the MySQL server. Remember this password, as it will be required to access the MySQL server.
   - Optionally, you can create additional user accounts.

6. Windows Service:
   - Choose to run MySQL as a Windows service. You can also set the service to start automatically.

7. Apply Configuration:
   - Click "Execute" to apply the configuration settings.

 Step 4: Verify Installation

1. Open MySQL Workbench:
   - After the installation and configuration are complete, open MySQL Workbench.

2. Connect to MySQL Server:
   - Create a new connection using the root account and the password you set during the configuration.
   - Test the connection to ensure it is working properly.

3. Run a Test Query:
   - In MySQL Workbench, run a simple test query to verify everything is set up correctly:
     ```sql
     SELECT VERSION();
     ```
   - This query should return the version of the MySQL server.



7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.
   Setting up development environments and using virtualization tools like Docker 

Step 1: Install Docker

1. Download Docker Desktop:
   - Go to the [Docker Desktop download page](https://www.docker.com/products/docker-desktop).
   - Download the Docker Desktop installer for Windows.

2. Install Docker Desktop:
   - Run the installer.
   - Follow the installation instructions, which typically involve agreeing to terms and setting some initial configurations.
   - Docker Desktop requires Windows 10 or later with the WSL 2 (Windows Subsystem for Linux) backend. The installer will guide you through setting this up if necessary.

3. Start Docker Desktop:
   - After installation, start Docker Desktop from the Start menu.
   - Docker will take a few moments to start up. You should see the Docker icon in your system tray when it's running.

Step 2: Verify Docker Installation

1. Open a terminal (Command Prompt, PowerShell, or Git Bash).
2. Run the following command to verify Docker is installed and running:
   ```bash
   docker --version
   ```
   This should return the version of Docker installed.

Step 3: Create a Dockerfile for Your Project

A `Dockerfile` is a script containing a series of instructions on how to build a Docker image for your application. Here’s an example `Dockerfile` for a simple Python application:

1. Create a `Dockerfile` in your project directory:
   ```Dockerfile
    Use an official Python runtime as a parent image
   FROM python:3.9-slim

    Set the working directory in the container
   WORKDIR /app

   #Copy the current directory contents into the container at /app
   COPY . /app

   #Install any needed packages specified in requirements.txt
   RUN pip install --no-cache-dir -r requirements.txt

   #Make port 80 available to the world outside this container
   EXPOSE 80

   Define environment variable
   ENV NAME World

   Run app.py when the container launches
   CMD ["python", "app.py"]
   ```

2. Create a `requirements.txt` file with your Python dependencies:
   ```txt
   Flask==2.0.1
   # Add other dependencies here
   ```

3. Create a simple `app.py` file:
   ```python
   from flask import Flask
   app = Flask(__name__)

   @app.route('/')
   def hello():
       return "Hello, World!"

   if __name__ == '__main__':
       app.run(host='0.0.0.0', port=80)
   ```

 Step 4: Build and Run Your Docker Container

1. Build the Docker image:
   ```bash
   docker build -t my-python-app .
   ```

2. Run the Docker container:
   ```bash
   docker run -p 4000:80 my-python-app
   ```
   - This runs the container and maps port 80 inside the container to port 4000 on your host machine.
   - You should be able to access the application by navigating to `http://localhost:4000` in your web browser.

Step 5: Use Docker Compose for Multi-Container Applications (Optional)

For more complex applications with multiple services (e.g., a web app with a separate database), Docker Compose can help manage multiple containers.

1. Create a `docker-compose.yml` file:
   ```yaml
   version: '3'

   services:
     web:
       build: .
       ports:
         - "4000:80"
     db:
       image: mysql:5.7
       environment:
         MYSQL_ROOT_PASSWORD: example
   ```

2. Start the services:
   ```bash
   docker-compose up
   ```




8. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.

9. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process. 

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
