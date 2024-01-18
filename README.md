-
































2nd Aug 2023

DevOps


●	DevOps is a set of practices that works to automate and integrate the processes between software development and IT(Operations) teams, so they can build, test, and deploy software faster and more reliably.

Application

●	An application is a computer program(Java/Python etc) that is designed for a particular task typically to be used by end-users.


 

Application Infrastructure

●	Servers
●	Databases
●	Firewalls
●	Networking etc

DevOps Learning Curve

Operations

Manage Servers 

 






Buying Servers ?

●	Okay, as we got to know what servers are, now to work with them we need to BUY SERVERS.

 

●	Now instead of buying servers, will RENT SERVERS on CLOUD.


 



Cloud Computing 

●	‘The Cloud’ can also refer to Cloud computing is the on-demand availability of compute power(Servers), database storage, applications, and other IT resources through a cloud services platform (AWS, AZURE etc) via the internet with pay-as-you-go pricing.

 





 

1.	Cloud AWS / Azure (LABS)
2.	Linux Basics
3.	Application Stack - PERN
4.	Application LMS ( Development )











3rd Aug 2023

AWS Cloud Account Setup

●	Visit - https://aws.amazon.com/free


●	Click the button to “Create an AWS Account”

●	On the next page, provide your Email Address, Password, and AWS Account Name (you can change this name in your account settings after sign up).

●	Click “Continue” to proceed
 
●	Next, you’ll provide your contact information. If you’re registering as an individual, select “Personal” and if you’re using any business, select “Company”

●	Complete the remaining fields with your information. Then click “Create Account and Continue” to proceed.


 

●	Next, you’ll be asked to provide a credit card for your AWS Account.

●	Once you’ve completed this information, click the “Secure Submit” button to proceed.

●	Next, you’ll be asked to complete a brief phone verification step. Here, you are asked to provide a phone number where you can be reached, and to click the “Call Me Now” button to receive an automated phone call.

●	Once you receive the call, you’ll input the number shown on your screen using your dial-pad
   



 
 



 





AZURE Account Setup - LABS


●	To start using the services we need an Azure Account

●	To create an Azure Account, we need a Phone Number, Email ID & Credit Card.

>  For 1st month Azure provides a Free Trial Subscription credits worth of $ 200 i.e Rs 14,500




> Search for create an azure account > 
 

●	Click on this URL, and here click on the Start free button.
 


 




 


 

 


Azure Portal

●	https://portal.azure.com

 
Azure VMS ( Virtual Machines )


●	I want you to picture an AZURE VM like a computer, and the components that make it up like OS, CPU, HDD, NW, Firewall, RAM etc.
 

 


SSH - Secure Shell

●	Secure Shell is a cryptographic network protocol for operating network services securely over an unsecured network.

●	Typical applications include login and remote command execution.

●	The default port for SSH client connections is 22.

 

 






7th Aug 2023
Azure VM Setup 
Create AZURE VM

●	Azure virtual machines (VMs) can be created through the Azure portal. The Azure portal is a browser-based user interface to create Azure resources. This quickstart shows you how to use the Azure portal to deploy a Linux virtual machine (VM) running Ubuntu 20.04 LTS. To see your VM in action, you also SSH to the VM.

1.	Enter virtual machines in the search.
2.	Under Services, select Virtual machines.
3.	In the Virtual machines page, select Create and then Virtual machine. The Create a virtual machine page opens.
4.	In the Basics tab, under Project details, make sure the correct subscription is selected and then choose to Create new resource group. Enter myResourceGroup for the name.*.
5.	Under Instance details, enter myVM for the Virtual machine name, and choose Ubuntu 20.04 LTS - Gen2 for your Image. Leave the other defaults. The default size and pricing is only shown as an example. Size availability and pricing are dependent on your region and subscription.
 

 

●	Click Review + Create














SSH Clients

●	An SSH client is a software program which uses the secure shell protocol to connect to a remote computer(AZURE/AWS server).

●	Examples - GitBash / Putty / Terminal (Visual Studio Code) etc

●	NOTE - If you have a Mac or Linux, you will then already have TERMINAL installed. 

SSH with PASSWORD

ssh username@public-ip-address

To connect remotely to a server via SSH, you can use the following command: ssh username@public-ip-address. This command initiates a secure shell connection to the server, allowing you to execute various commands and interact with the server's file system. You may need to provide additional authentication credentials, such as a password.









8th Aug 2023

AWS EC2 ( Elastic Compute Cloud )

●	Amazon Elastic Compute Cloud is a part of Amazon.com's cloud-computing platform, Amazon Web Services, that allows users to rent virtual computers(Servers/Machines) on which to run their own computer applications.

 


AWS EC2 Instance Setup 

●	NOTE : AWS Supports Only KEY BASED AUTHENTICATION


Brute Force Attack

 













Key Pairs 

●	A key pair, consisting of a public key and a private key, is a set of security credentials that you use to prove your identity when connecting to a Server.

 
SSH without PASSWORD (Key Based Authentication)
 

chmod 400 file.pem 

●	The command "chmod 400" is used to set the file's permission to be readable only by the owner of the file.

ssh -i private-key.pem username@public-ip-address



9th Aug 2023

Operating Systems

●	An operating system (OS) is a software that manages SERVER (AWS/AZURE/etc) hardware.

●	The main purpose of an operating system is to provide an environment in which a user can execute programs in a convenient and efficient manner.


 





Ubuntu
○	Ease of use
○	Modern software packages
○	Based on Debian
○	Released every six months
○	Large community of users and developers

If you want access to the latest software and a more user-friendly environment, Ubuntu may be a better fit.
Linux Architecture

 


💡 Kernel: Central module(Heart) of OS, interacts with Hardware and responsible for memory management, process management etc.

uname -r

The uname -r command is used for displaying kernel version


💡 Shell : Shell is a command line interpreter i.e, translates commands entered by the user and converts them into a language that is understood by Kernel. 

printenv
echo $SHELL

BASH
In order to execute commands in Ubuntu, one can use the Bash shell. The Bash shell is a command-line interface that allows users to interact with the Ubuntu operating system through a series of text commands.





Understanding Command Line Interface - CLI

The Command Line Interface (CLI) is a powerful tool for interacting with computers(Servers), through text-based commands. 

💡 Additionally, the CLI can be a valuable tool for automating repetitive tasks and performing complex operations that would be difficult or impossible to accomplish through graphical user interfaces (GUIs).

CLI == 100% AUTOMATION












Understanding Linux File System
The Linux directory structure is like a tree. The base of the Linux file system hierarchy begins at the root (/). Directories branch off the root, but everything starts at root.


 


sudo

The sudo command stands for “super user do!”

If you prefix “sudo” with any linux command, it will run that command with elevated privileges.  Elevated privileges are required to perform certain administrative tasks. 

sudo command 
whoami
sudo whoami

Someday you may wish to run an Apache Web Server or MYSQL Database server and have to manually edit your config files. You might also have to restart the Web Server or Database services, then you need elevated privileges.

If you are familiar with Windows, if you try to perform an administrative task, a dialog box asks you if you wish to continue ? The task is then performed.   
 



10th Aug 2023
vi editor

The vi editor is a powerful and versatile text editor that comes pre-installed on most Unix-based systems, including Ubuntu
To launch the vi editor

vi file.txt

Some of the commonly used vi editor commands include:
●	i command: This command is used to enter the insert mode, which allows the user to insert new text at the cursor position.
●	w command: This command is used to write the current file to disk.
●	q command: This command is used to quit the vi editor.
●	:wq command: This command is used to write the current file to disk and quit the vi editor







File & Directory Management
The commands that can be used to create, delete, move, and modify files and directories.
cp command
The cp command in Linux, which is used to copy files and directories from one location to another.
●	File Copying
cp filename.txt filename_backup.txt
Simply use the command cp filename.txt filename_backup.txt to create a copy of the file with the name "filename_backup.txt".

●	Directory Copying
cp -r /home/user/documents /home/user/backup
●	Another useful feature of the cp command is the ability to copy entire directories. To do this, use the -r option followed by the directory name.

●	cp -r The r flag specifies that the copy should be done recursively, meaning that all subdirectories and their contents will also be copied.





SCP
SCP - Secure Copy, used for remotely copying files & directories across servers / local machines etc

PASSWORD 
scp source_filename.txt <username>@<public-ip>:~

PASSWORDLESS / KEYBASED

ssh -i private-key.pem username@public-ip-address

scp -i private-key.pem  source_filename.txt <username>@<public-ip>:~














rm command
The rm command command in Unix and Linux systems can remove files and directories, but should be used with caution to avoid unintended data loss. 
●	File Removal
rm file.txt
For example, let's say you have a file called "file.txt" located in your current working directory. To delete this file, you would use the command rm file.txt.
●	
rm -f file.txt

●	Directory Removal
rm -r directory
●	If you want to delete a directory and all its contents, you can use the command rm -r directory. This will delete the specified directory and all its contents.




mv command
The mv command is a powerful tool in the Unix/Linux command line that allows you to move files or directories from one location to another. It works by taking two arguments: the first is the source file or directory, and the second is the destination.
●	Move
For example, let's say you have a file named file.txt in your current directory, and you want to move it to a subdirectory called archive. You can use the mv command like this:
mv file.txt archive

In addition to moving files or directories, mv can also be used to rename files and directories. Simply use the original name as the source, and the new name as the destination.
●	Rename
mv [current_file_name] [new_file_name]







Archive Files Using tar and zip utilities
tar zip and unzip command

The tar, zip, and unzip commands are used for file compression and decompression.
The tar command is used to create a single archive file from multiple files, 

tar cvf FILENAME.tar DIRECTORY/
The above command creates a tar archive of the specified directory. The tar command is used to compress and archive files and directories. The "-c" option tells tar to create a new archive, the "-v" option enables verbose output, and the "-f" option specifies the filename of the archive. 

tar xvf FILE.tar
The command "tar xvf FILE.tar" is used to extract files from an archive. The "-x" option specifies that the files should be extracted, while the "-v" option displays each file as it is processed. The "-f" option is used to specify the archive file to be extracted, which in this case is "FILE.tar".





11th Aug 2023
Installations

 

Installation methods 

zip
man dpkg
dpkg -l
dpkg -l | grep git
dpkg -l | grep java
ls
wget http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0-11build1_amd64.deb
ls
dpkg -i zip_3.0-11build1_amd64.deb
sudo dpkg -i zip_3.0-11build1_amd64.deb
zip


unzip
apt install unzip
sudo apt install unzip
unzip


kubectl
sudo apt install kubectl
sudo snap install kubectl
wget https://s3.us-west-2.amazonaws.com/amazon-eks/1.27.1/2023-04-19/bin/linux/amd64/kubectl
./kubectl
chmod +x kubectl
./kubectl



package management

Package management in Linux involves the process of installing, updating, configuring, and removing software packages. It is a crucial aspect of maintaining a Linux system and ensuring that all necessary software components are installed and up-to-date. Package management tools such as dpkg, apt-get, yum, and pacman are used to manage packages in various Linux distributions. 
APT command
APT command is a powerful tool used for managing packages on Linux systems. It provides an efficient and effective way of installing, updating, and removing software packages, as well as resolving dependencies between them.
Install & Update

sudo apt -y install package
To install the package, you can use the command sudo apt -y install package. This command will download and install the necessary files for the package. After it is installed, you can start using the package by calling its functions in your code. It is important to note that you should always make sure to use the most updated version of the package, as this will ensure that you have access to all the latest features and bug fixes. You can check for updates by running the command sudo apt update before installing the package.

sudo apt -y install zip





unzip FILE.zip
The above command is used to extract the contents of a compressed ZIP file. Once the file is unzipped, the contents can be accessed and used. When unzipping the file, the command will create a new folder with the same name as the ZIP file, containing all the contents of the ZIP file inside.





180  zip
  181  unzip
  182  java
  183  zip
  184  man dpkg
  185  dpkg -l
  186  dpkg -l | grep git
  187  ls
  188  vi file.txt
  189  grep file file.txt
  190  dpkg -l | grep java
192  ls
  193  wget http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0-11build1_amd64.deb
  194  ls
  195  dpkg -i zip_3.0-11build1_amd64.deb
  196  sudo dpkg -i zip_3.0-11build1_amd64.deb
  197  zip
206  zip text-files.zip *.txt
  207  ls
  208  rm *.txt
  209  ls
  210  unzip
  211  man apt
  212  apt install unzip
  213  sudo apt install unzip
  214  unzip
  215  ls
  216  unzip text-files.zip
  217  ls
  218  kubectl
  219  sudo apt install kubectl
  220  sudo snap install kubectl
  221  kubectl
225  ls kubectl
  226  ls
  227  wget https://s3.us-west-2.amazonaws.com/amazon-eks/1.27.1/2023-04-19/bin/linux/amd64/kubectl
  228  ls
  229  ./kubectl
  230  chmod +x kubectl
  231  ls
  232  ./kubectl
1  uname
    2  printenv
    3  ls
    4  pwd
    5  mkdir new-folder
    6  ls
    7  touch new-file.txt
    8  ls
    9  cp new-file.txt backup.txt
   10  ls
   11  echo hello
   12  zip
   13  unzip
   14  tar
   15  ls
   16  tar cvf file.tar *.txt
   17  ls
   18  zip
   19  unzip
   20  wget
   21  curl
   22  curl -O http://mirror.centos.org/centos/7/os/x86_64/Packages/zip-3.0-11.el7.x86_64.rpm
   23  ls
   24  rpm -l
   25  rpm -qa
   26  rpm -qa | grep unzip
   27  rpm -qa | grep python
   28  ls
   29  sudo rpm -ivh zip-3.0-11.el7.x86_64.rpm
   30  zip
   31  ls
   32  zip files.zip *.txt
   33  ls
   34  unzip
   35  yum install unzip
   36  sudo yum install unzip
   37  unzip
   38  ls
   39  rm *.txt
   40  ls
   41  unzip files.zip
   42  ls
   43  curl -O https://s3.us-west-2.amazonaws.com/amazon-eks/1.27.1/2023-04-19/bin/linux/amd64/kubectl
   44  ls
   45  chmod +x kubectl
   46  ./kubectl




14th Aug 2023

sudo vi /etc/passwd
sudo vi /etc/shadow
sudo passwd ubuntu
sudo systemctl restart sshd
sudo vi /etc/ssh/sshd_config
id john
sudo adduser john
chmod ugo-r kubectl
ls -l kubectl
chmod ugo+r kubectl
cp kubectl /tmp
sudo vi /etc/group
sudo usermod -aG ubuntu john
chmod o+x kubectl
ls -l kubectl
chmod 444 kubectl
ls -l kubectl
chmod 664 kubectl

USER Management
It involves creating, modifying, and deleting user accounts and groups on the system. To create a new user account, the administrator must provide a username and password.


sudo adduser username

To create a new user in the Linux terminal, you can use the command sudo adduser username. This command will prompt you to enter a password for the new user and some additional information, such as their full name and phone number. Once you have entered this information, the new user will be added to the system and will be able to log in and use the terminal. It is important to note that you should choose a strong password for the new user to ensure the security of your system.

sudo usermod <options>

sudo userdel <options>






File Permissions
When it comes to file permissions in Ubuntu, there are a few key things to keep in mind. Firstly, Ubuntu uses a permissions system to determine who is allowed to view, edit, or execute specific files. This system is based on the concept of users and groups, with each file being assigned a set of permissions that specifies which users or groups are allowed to perform which actions.

Symbolic Mode Permissions
There are three options for permission groups available to you in Linux. These are
owners: these permissions will only apply to owners and will not affect other groups.
groups: you can assign a group of users specific permissions, which will only impact users within the group.
all users(others): these permissions will apply to all users, and as a result, they present the greatest security risk and should be assigned with caution.
There are three kinds of file permissions in Linux:
Read (r): Allows a user or group to view a file.
Write (w): Permits the user to write or modify a file or directory.
Execute (x): A user or group with execute permissions can execute a file or view a directory.
The command for changing directory permissions for group owners is similar, but add a “g” for group or “o” for users:

chmod o+w filename
chmod o+r filename
chmod o-w filename

Absolute Mode Permissions
The permissions can also be represented by numbers, with 4 indicating read access, 2 indicating write access, and 1 indicating execute access.
To use this command, you need to specify the desired permissions as a three-digit number, where each digit corresponds to a specific group of users (owner, group, and others, respectively).
For example, if you want to give read and execute access to the owner of a file, write access to the group, and no access to others, you would use the command "chmod 750 file.txt". Here, 7 represents read, write, and execute access for the owner (4+2+1), 5 represents read and execute access for the group (4+1), and 0 represents no access for others.

chmod 664 filename
chmod 660 filename
chmod 400 filename







16th Aug 2023
Application

●	An application is a computer program(Java/Python etc) that is designed for a particular task typically to be used by end-users.

Three Tier Architecture
The three tier architecture is a widely used architectural pattern that divides an application into three interconnected layers: the presentation layer, the application layer, and the data layer.

💡 The presentation layer is responsible for displaying the user interface and receiving user input.

💡 The application layer contains the business logic and processes the user input.

💡 Finally, the data layer is responsible for storing and retrieving data used by the application.

 

This architecture provides a number of benefits, such as scalability, maintainability, and flexibility. By separating the user interface, the business logic, and the data storage, developers can easily modify or replace one layer without affecting the others.
Application Stack
An application stack is a set of software programs that work together to support the development and operation of an application. 
This can include software for the front-end or user interface, the back-end or server-side, and the database.
It's important to choose the right application stack for your needs, as different stacks have different strengths and weaknesses depending on the type of application you're building, the programming language you're using, and other factors. 



Most Popular Stacks
https://en.wikipedia.org/wiki/Programming_languages_used_in_most_popular_websites

LMS - Learning Management System
A Learning Management System (LMS) is a software application used for the administration, documentation, tracking, reporting, and delivery of educational courses, training programs, or learning and development programs. 
 

💡 Visit - https://lms.digital-lync.com/

LMS Uses three tier architecture 
Frontend 
 

 


Backend + Database
 

 

LMS - Application Stack

Database
A database is a collection of data that is organised in a way that allows it to be easily accessed, managed, and updated. 
 
SQL (Structured Query Language) is a programming language which is used to manage data stored in relational databases like MySQL, MS Access, SQL Server, Oracle, Sybase, Informix, Postgres etc.
Postgres
Postgres, also known as PostgreSQL, is a powerful and popular open-source relational database management system. Postgres is known for its robustness, extensibility, and adherence to SQL standards.



Backend
The term 'backend' refers to the part of a software application that is responsible for handling the server-side processing. This includes the server, and the application logic that handles data and user requests. 
Nodejs
Node.js is a JavaScript runtime environment used by developers to build scalable network applications. Nodejs handles large volumes of connections with low latency and offers a vast library of modules through npm. With its growing popularity, Node.js has become an essential tool for modern web development.

Frontend
The frontend is a crucial part of any software application, as it is the part that users interact with directly. It encompasses the user interface, which includes elements such as buttons, forms, and menus
Reactjs
ReactJS is a popular JavaScript library that is commonly used to build user interfaces. It was created by Facebook and has gained widespread adoption due to its ability to enable developers to create complex, interactive applications with ease. 




SDLC  - Software Development Life Cycle
The Software Development Life Cycle (SDLC) is a process followed by software development teams to design, develop, and test high-quality software. 
The SDLC consists of multiple stages such as Analysis, Design, Code, Build, Test, Release, and Deploy.
 











17th Aug 2023

LMS Application Lifecycle
 


 


 







18th Aug 2023
Version Control System - VCS

VCS helps software teams to manage and track changes made to the source code. Version control is a crucial aspect of the DevOps role. 

Version control / Revision control / Source control is a system that helps to keep track of changes made to a file or a set of files(computer programs, web site files, documents etc) over time.
💡 Why do we need VCS ?
 Version control gives the ability to revert a document to a previous version.
 






●	You can think of a version control system ("VCS") as a kind of "database".

●	In VCS terminology we call it as “REPOSITORY”

 

Repository

Repositories are used to store different types of files including code, images, documents, among others. They are commonly used in software development to manage code and track changes made by different contributors(developers).





Commits
When a developer makes changes to a codebase, they create a new version of the codebase, called a commit. This commit essentially records the state of the codebase at a particular point in time. It includes the changes made by the developer, as well as a commit message that describes the changes made.

Centralised vs Distributed 

 




 

 
Introduction GitHub
GitHub is a web-based platform that provides users with a wide range of tools and resources to help them manage and collaborate on software projects. Through GitHub, users can share code, track changes, manage projects, and collaborate with others in real-time. 

 
GitHub Repository

●	A repository contains all of your project's files and each file's revision history. You can discuss and manage your project's work within the repository.

●	You can own repositories individually, or you can share ownership of repositories with other people in an organization.

Create Repo
●	Create GitHub Account - https://github.com/

 






 














21st Aug 2023
IDE
 

●	An Integrated Development Environment is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of at least a source code editor, build automation tools and a debugger.
 


Setting the git Configuration

git config --global user.name "ravi2krishna"
git config --global user.email "ravi2krishna@gmail.com"


Using existing GIT Repositories with Clone
Using GIT Repositories with Clone
When you create a clone of a repository, you create a copy of the entire repository on your local machine. This means that you have all the files and directories that make up the project, as well as the entire version history. You can make changes to the project, commit those changes, and then push them back up to the main repository.
 

Git Workflow
 

Git architecture also includes a staging area, which acts as an intermediate step between the working directory and the repository. This allows developers to selectively choose which changes to commit.

 

 



 
GIT PUSH

●	Use git push to push commits made on your local repository to a remote repository.

●	The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo.

 









PAT - Personal Access Token

●	PAT - Personal Access Token for HTTPS

●	https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token


 

 

 
 

 

●	Copy the token and paste token







22nd Aug 2023
Git CLI Workflow

CLI Workflow

	
cd repository
git status                   	
vi index.html   
       { put some content }               
git status
git add index.html   
       { staged the changes }
git commit -m "Create Index Page"    
       { Committed from staging area to local repo}
git status
git push


●	The git add command - adds a change in the working directory to the staging area. It tells Git that you want to include updates to a particular file in the next commit. 

●	The git commit command - creates a commit, which is like a snapshot of your repository. These commits are snapshots of your entire repository at specific times. You should make new commits often, based around logical units of change. Over time, commits should tell a story of the history of your repository and how it came to be the way that it currently is. Commits include lots of metadata in addition to the contents and message, like the author, timestamp, and more.
○	 git commit -m "descriptive commit message"

●	The git push command - The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo.

BRANCHES

●	In a collaborative environment, it is common for several developers to share and work on the same source code. Some developers will be fixing bugs while others would be implementing new features. Therefore, there has got to be a manageable way to maintain different versions of the same code base.

●	Branch allows each developer to branch out from the original code base and isolate their work from others.

●	Branching means you diverge from the main line(master - working copy of application) of development and continue to do work without messing with that main line.


 


 







Creating a branch

1.	On GitHub.com, navigate to the main page of the repository.
2.	Optionally, if you want to create your new branch from a branch other than the default branch for the repository, click  NUMBER branches then choose another branch:
3.	Click the branch selector menu.
4.	 
5.	Type a unique name for your new branch, then select Create branch.
 
 

Deleting a branch

●	Note: If the branch you want to delete is the repository's default branch, you must choose a new default branch before deleting the branch

1.	On GitHub.com, navigate to the main page of the repository.
2.	Above the list of files, click  NUMBER branches.
3.	 
4.	Scroll to the branch that you want to delete, then click .
5.	 

Create Branch CLI

●	When you create a new branch, git creates a new pointer for you to move around.

●	To view branches

git branch

●	Let’s say you create a new branch called feature_payment

git branch feature_payment
git branch

Switching Branches

●	To switch between branches, you can use git checkout command

git checkout feature_payment
git branch
git status

 

 


Merging

●	The git merge command lets you take the independent lines of development created by the git branch and integrate them into a single branch.

●	Git merge will combine multiple sequences of commits into one unified history. In the most frequent use cases, git merge is used to combine two branches. 

git checkout main
git merge feature_payment

 

Delete Branch CLI

●	Delete a branch on your local filesystem :

git branch feature_support
git branch 
git branch -d <branch_name>
git branch -d feature_support







 












Pushing Changes

 

 

 

 

 

 


Collaborate 


 

 

 

 

 


 

 

 

 

 

 

 

 

 
















PULL REQUEST


●	Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.

●	After initializing a pull request, you'll see a review page that shows a high-level overview of the changes between your branch (the compare branch) and the repository's base branch.

●	After you're happy with the proposed changes, you can merge the pull request. If you're working in a shared repository model, you create a pull request and you, or someone else, will merge your changes from your feature branch into the base branch you specify in your pull request.

Pull Request Flow

Creating a repository
A repository is usually used to organize a single project. Repositories can contain folders and files, images, videos, spreadsheets, and data sets -- anything your project needs. Often, repositories include a README file, a file with information about your project. GitHub makes it easy to add one at the same time you create your new repository. It also offers other common options such as a license file.
Your hello-world repository can be a place where you store ideas, resources, or even share and discuss things with others.
1.	In the upper-right corner of any page, use the  drop-down menu, and select New repository.
2.	 
3.	In the Repository name box, enter hello-world.
4.	In the Description box, write a short description.
5.	Select Add a README file.
6.	Click Create repository.
7.	 
Creating a branch
Branching lets you have different versions of a repository at one time.
By default, your repository has one branch named main that is considered to be the definitive branch. You can use branches to experiment and make edits before committing them to main.
When you create a branch off the main branch, you're making a copy, or snapshot, of main as it was at that point in time. If someone else made changes to the main branch while you were working on your branch, you could pull in those updates.
This diagram shows:
●	The main branch
●	A new branch called feature
●	The journey that feature takes before it's merged into main
 
Have you ever saved different versions of a file? Something like:
●	story.txt
●	story-joe-edit.txt
●	story-joe-edit-reviewed.txt
Branches accomplish similar goals in GitHub repositories.
Here at GitHub, our developers, writers, and designers use branches for keeping bug fixes and feature work separate from our main (production) branch. When a change is ready, they merge their branch into main.
Create a branch
1.	Click the Code tab of your hello-world repository.
2.	Click the drop down at the top of the file list that says main.
3.	 
4.	Type a branch name, readme-edits, into the text box.
5.	Click Create branch: readme-edits from main.
 
Now you have two branches, main and readme-edits. Right now, they look exactly the same. Next you'll add changes to the new branch.
Making and committing changes
When you created a new branch in the previous step, GitHub brought you to the code page for your new readme-edits branch, which is a copy of main.
You can make and save changes to the files in your repository. On GitHub, saved changes are called commits. Each commit has an associated commit message, which is a description explaining why a particular change was made. Commit messages capture the history of your changes so that other contributors can understand what you’ve done and why.
1.	Click the README.md file.
2.	Click  to edit the file.
3.	In the editor, write a bit about yourself.
4.	In the Commit changes box, write a commit message that describes your changes.
5.	Click Commit changes.
6.	 
These changes will be made only to the README file on your readme-edits branch, so now this branch contains content that's different from main.
Opening a pull request
Now that you have changes in a branch off of main, you can open a pull request.
Pull requests are the heart of collaboration on GitHub. When you open a pull request, you're proposing your changes and requesting that someone review and pull in your contribution and merge them into their branch. Pull requests show diffs, or differences, of the content from both branches. The changes, additions, and subtractions are shown in different colors.
As soon as you make a commit, you can open a pull request and start a discussion, even before the code is finished.
By using GitHub's @mention feature in your pull request message, you can ask for feedback from specific people or teams, whether they're down the hall or 10 time zones away.
You can even open pull requests in your own repository and merge them yourself. It's a great way to learn the GitHub flow before working on larger projects.
1.	Click the Pull requests tab of your hello-world repository.
2.	Click New pull request
3.	In the Example Comparisons box, select the branch you made, readme-edits, to compare with main (the original).
4.	Look over your changes in the diffs on the Compare page, make sure they're what you want to submit.
5.	 
6.	Click Create pull request.
7.	Give your pull request a title and write a brief description of your changes. You can include emojis and drag and drop images and gifs.
8.	Click Create pull request.
Your collaborators can now review your edits and make suggestions.
Merging your pull request
In this final step, you will merge your readme-edits branch into the main branch.
1.	Click Merge pull request to merge the changes into main.
2.	Click Confirm merge.
3.	Go ahead and delete the branch, since its changes have been incorporated, by clicking Delete branch.

 









Branch Protection Rule

https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule


24th Aug 2023

Merge Pull Request

●	Merge a pull request into the upstream branch when work is completed. Anyone with push access to the repository can complete the merge.

●	In a pull request, you propose that changes you've made on a head branch should be merged into a base branch. By default, any pull request can be merged at any time, unless the head branch is in conflict with the base branch. However, there may be restrictions on when you can merge a pull request into a specific branch. For example, you may only be able to merge a pull request into the default branch if required status checks are passing. For more information, see "protected branches."

1.	Under your repository name, click  Pull requests.
2.	 
3.	In the "Pull Requests" list, click the pull request you'd like to merge.
4.	Depending on the merge options enabled for your repository, you can:
○	Merge all of the commits into the base branch by clicking Merge pull request. If the Merge pull request option is not shown, then click the merge drop down menu and select Create a merge commit.
○	 













 

Merge vs Rebase

Merge - maintain complete history
Rebase - clean history only

> Merge will generally create an extra commit 
> Rebase rewrites history,

> It depends on what is most important - a tidy history or a true representation of the sequence of development

25th Aug 2023
Undoing

Testing For DevOps

Testing for DevOps is a crucial aspect of software development that cannot be overlooked. It involves ensuring that the software is functioning optimally and reliably in the production environment.

SonarQube

●	SonarQube is an open source platform developed by SonarSource for continuous inspection of Code Quality

●	SonarQube offers reports on duplicated code, coding standards, unit tests, bugs and security vulnerabilities.




 

 


●	SonarQube is a Java application that requires a Java Web Runtime Environment.
Setting Up SonarQube

 


28th Aug 2023


●	SonarQube Requires “t2.large instance” i.e 8 GB RAM - 2 CPU’s on AWS, with 30 GB as Storage.

●	SonarQube works on “port 9000”, make sure to add port 9000 as part of your Security Group
Install Docker

Simple Script to Install Docker Software

docker
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
docker

Install SonarQube With Docker


sudo ss -ntpl
sudo docker container run -dt --name sonarqube -p 9000:9000 sonarqube
sudo ss -ntpl


○	Default credentials are 
■	Username is admin 
■	Password is admin

After stopping EC2 server, to start sonarqube again use following command
sudo docker container start sonarqube 

SonarQube & Sonar Scanner
Sonar Scanner and SonarQube are two powerful tools used for static code analysis. These tools are designed to provide developers with a comprehensive view of the quality of their code, including areas that need improvement. 
●	Sonar Scanner is a command-line tool that performs code analysis
●	SonarQube is a web-based platform that gives dashboard
 





LMS App CODE

> git clone -b dev https://github.com/ravi2krishna/lms.git

IMPORTANT Fork Above Project to your Github Accounts

Perform Code Analysis on LMS App

Make sure to change the username here from ravi2krishna to your username

ls
git clone -b dev https://github.com/ravi2krishna/lms.git
ls
cd ~/lms/webapp
ls
sudo docker run  --rm -e SONAR_HOST_URL="http://3.19.219.206:9000" -e SONAR_LOGIN="sqp_e9b5887342f2740c3d9746367abf42aedc97e4ca"  -v ".:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey=lms


 




















29th Aug 2023 

Software Build

●	The term build may refer to the process by which source code is converted into a binary artifact ( binary code / executable code).


●	Source Code == Human Readable Code [ ENGLISH ]
●	Binary / Executable Code == Machine Readable Code [ 0’s and 1’s ]

 




●	Builds vary based on technologies used.

●	When we are working with Java Applications, we will use a build software called called “MAVEN”

Any Build Implementation


●	Source Code Files 
○	Source code is the list of human-readable instructions that a programmer writes often in a word processing program when he is developing a program.

●	Metadata File
○	It is a file that contains information about the project and configuration details used to build the project. 

●	Testing Code
○	Software Testing is a method to check whether the actual software product matches expected requirements and to ensure that software product is Defect free. 

●	After Build - Binary Code 
○	Build artifacts are files produced by a build.
○	As DevOps Engineer, you need to understand this.








Building Java Application

> https://github.com/ravi2krishna/JavaCalculator.git

> Build the following application by fetching code from “qa” branch



cd ~
git clone -b qa https://github.com/ravi2krishna/JavaCalculator.git
sudo apt -y install openjdk-11* maven
cd ~/JavaCalculator
ls target
mvn package
ls 
ls target
java -jar target/*.jar 10 20
java -jar target/*.jar 40 50















Building LMS Application


●	LMS App Requires Following Rules in Security Group
○	SSH - 22- Login
○	DATABASE TIER [ POSTGRES ] - 5432 - Storing Data
○	APPLICATION TIER [ NODEJS ] - 8080 - Business Logics
○	FRONTEND TIER [ REACTJS ] { Hosted Web Server } - 80/443 
LMS Architecture
 
30th Aug 2023 

Setup Database LMS

Install postgres 

> Goto https://www.postgresql.org/download/linux/ubuntu/
> By running the Below 4 commands you can install the postgres

sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'

The command above is a Bash command that adds a new repository to the list of available repositories for the Advanced Package Tool (APT). Specifically, it adds the PostgreSQL Global Development Group (PGDG) repository to the list. The sudo command is used to run the command with elevated privileges, allowing the user to modify system files. The sh -c option runs the command following it, enclosed in quotes, in a new shell instance. The echo command is used to print the specified text to the standard output, which is then redirected to a new file located at /etc/apt/sources.list.d/pgdg.list, creating the file if it does not exist or overwriting it if it does. This new file will contain the line deb <http://apt.postgresql.org/pub/repos/apt> $(lsb_release -cs)-pgdg main, which specifies the location of the PGDG repository.
It is important to note that the $(lsb_release -cs) part of the command is a Bash command substitution that evaluates to the codename of the current Ubuntu release. This ensures that the correct version of the PGDG repository is added to the APT sources list.


sudo apt install wget -y

The above command is used to install the wget package in a Linux operating system.
wget is a utility for downloading files from the web. It is often used to automate the download of files from websites. It is commonly used in scripts and command-line tools to download files without the need for a graphical interface.

wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -

The command above is used to download the PostgreSQL repository signing key and add it to the system's keyring. The "wget" command is used to download the key, while the "-O -" option is used to output the downloaded content to the standard output stream. The content is then piped to the "sudo apt-key add -" command, which adds the key to the system's keyring. The "apt-key" command is used to manage authentication keys for Debian-based systems, allowing the system to verify the authenticity of packages downloaded from the repository. This command is often used when installing PostgreSQL on a Linux system.


sudo apt-get update -y

To ensure that your system is up-to-date, you can run the above command.





sudo ss -ntpl
sudo apt-get -y install postgresql
sudo ss -ntpl

This command downloads and installs PostgreSQL on the system. After installation, the user can run various commands to create and manage PostgreSQL databases, tables, and users, depending on their needs.

Once we installed postgres we need to set the password for the postgres database.

Set Password - postgres 

Commands to set the password for postgres

sudo su - postgres

To gain superuser access to the PostgreSQL database system, you can use the command sudo su - postgres in your terminal. 


psql

When working with PostgreSQL, one way to interact with the database is by using the command-line interface called "psql".


Set the password using following command
\password
\q
exit


Comparison with Java

 







Setup Backend For LMS

To install Node.js version 16 on your system, you can run the following command in your terminal:
node -v
npm -v


curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -

sudo apt-get install -y nodejs

The above command will install Node.js on your system 
node -v

To check the version of Node.js installed on your computer, you can use the command "node -v"

npm -v

Running the command npm -v will display the version of npm
With npm, you can search for packages to add to your project, install specific versions of packages, and manage your project's dependencies with ease.





Build LMS Backend Application

Change the directory to api, Then create a .env file in the api folder which is our backend source code, where we would specify the database connection details.

cd ~/lms/api
vi .env

MODE=production
PORT=8080
DATABASE_URL=postgresql://postgres:Admin123*@localhost:5432/postgres


Run the following commands to build the Application, which will create build folder, in which our application will be made available

npm install
sudo npm install -g pm2
sudo npx prisma db push
ls build
npm run build
ls build










Start Backend Application
sudo ss -ntpl
NODE_PORT=8080 pm2 start -i 0 build/index.js
sudo ss -ntpl

In order to start the application, the command "NODE_PORT=8080 pm2 start -i 0 build/index.js" is used. This command is used to launch the application with the specified port number and with a process manager that ensures that the application is always running. The "NODE_PORT" variable specifies the port number to be used for the application. In addition, the "pm2" process manager is used to launch the application with the specified index file. The "-i 0" option specifies that the application should use as many processes as there are CPUs on the machine. This ensures that the application is able to handle a large number of requests without crashing.


Locally verify 
curl http://localhost:8080/api

{"message":"success","mode":"production"}

Verify with Browse - http://public-ip:8080/api
 
31st Aug 2023 
Build LMS Frontend 
Reactjs
ReactJS is a popular JavaScript library that is commonly used to build user interfaces.
Change the directory to webapp, Then create a .env file in the webapp folder which is our frontend source code, where we would specify the backend connection details.

cd ~/lms/webapp
vi .env

VITE_API_URL=http://public-ip:8080/api


Run the below commands to build the Application, which will create dist folder, in which our application will be made available
npm install
ls dist
npm run build
ls dist







Web Servers

WEB SERVER - A web server is computer software [ Nginx HTTP Server ] and underlying hardware  [ AWS Instance / AZURE VM ] that accepts requests via HTTP (port 80) / HTTPS (port 443)   to distribute web content.
 






Nginx Web Server
Nginx web server is a high-performance web server that is commonly used for serving static content such as images, videos, and CSS files. 
 








Setup Nginx Web Server
Nginx Web Server is not installed by default , the package name of Nginx HTTP Server is nginx and it runs on port 80.
sudo ss -ntpl
sudo systemctl status nginx

When troubleshooting issues related to web servers, it can be helpful to check the status of the server's processes. One way to do this is by using the command line interface and running the command sudo systemctl status nginx. This command will display information about the status of the Nginx web server, including whether it is running, any errors that may have occurred, and other diagnostic information.
sudo apt -y install nginx

Install Nginx by executing the command "sudo apt -y install nginx". This will automatically install Nginx and its dependencies. Once the installation is complete, you can configure Nginx to meet your specific needs. With Nginx installed, you can take advantage of its powerful features to host web applications, serve static files, or act as a reverse proxy. So, start using Nginx today and discover why it is one of the most popular web servers in the world!










Test Web Server
💡 Browse - http://public-ip
 

💡 If you are the website administrator: You may now add content to the directory DocumentRoot - /var/www/html/

The /var/www/html/ directory is a critical component of the file system in a Linux operating system. It is the default directory where web server files are stored, such as HTML, CSS, and JavaScript files. The files stored in this directory are accessible via a web browser and are used to render web pages. 

ls /var/www/html
vi /var/www/html/index.nginx-debian.html
sudo rm -rf /var/www/html/*
ls /var/www/html

The command "sudo rm -rf /var/www/html/* is used to delete the contents of the "/var/www/html/" directory in a Linux system.  

ls /var/www/html
sudo cp -r ~/lms/webapp/dist/* /var/www/html
ls /var/www/html
ls ~/lms/webapp/dist/

Test LMS Application
💡 Browse - http://public-ip

 








DNS

DNS is a critical component of the internet infrastructure, allowing human-readable domain names to be translated into machine-readable IP addresses and vice versa.

 


 



 

Production Setup
HTTP (HyperText Transfer Protocol) and HTTPS (HTTP Secure) are both protocols for sending data between a client and a server. 
 

Certbot
Certbot is a free and open-source software tool that is used for automatically configuring TLS encryption on a web server.
 The tool uses a plugin architecture to communicate with various web servers, such as Apache and Nginx, to automatically generate and install SSL/TLS certificates on your webserver. The software is designed to be easy to use, and its configuration is straightforward. 
 

Enable HTTPS
To make changes to your NGINX server, you can run the commands

sudo rm /etc/nginx/sites-enabled/default
sudo vi /etc/nginx/sites-available/lms-app

Here are the steps to edit the configuration file for your LMS app:
1.	This will open the configuration file in the Vi editor.


server {
server_name lms.vrkstech.com;

location / {
    root /var/www/html;
}

location /api {
    proxy_pass http://localhost:8080;
}

}


sudo ln -s /etc/nginx/sites-available/lms-app /etc/nginx/sites-enabled/lms-app

To enable the LMS app on your NGINX server, you can create a symbolic link between the /etc/nginx/sites-available directory and the /etc/nginx/sites-enabled directory. To do this, run the following command as a user with sudo privileges

sudo systemctl restart nginx





To install the core snap package and make sure it is up to date, simply enter the following command in your terminal:
sudo snap install core; sudo snap refresh core

Once the installation and refresh are complete, you will have access to a wide range of snap packages and features. These packages and features can greatly enhance the functionality and usability of your system, allowing you to streamline your workflow.


The process of installing Certbot can be done easily by entering the command:

sudo snap install --classic certbot

Once installed, you will be able to manage your website’s SSL certificates in a safe and secure manner, and ensure that your website and its users are protected from potential security threats. This makes managing your website’s SSL certificates a breeze, and allows you to focus on other important aspects of your website’s maintenance.

To create a symbolic link between /snap/bin/certbot and /usr/bin/certbot, you can use the command:
sudo ln -s /snap/bin/certbot /usr/bin/certbot


To install a free SSL certificate on your website, you can run the following command in your terminal:

sudo certbot --nginx

This command will use the Certbot tool to automatically request and install a certificate from Let's Encrypt, a free and open Certificate Authority. Additionally, Certbot will configure your Nginx web server to use the new certificate for secure HTTPS connections. After running this command, be sure to restart your Nginx server to apply the changes.

sudo systemctl restart nginx


 





Rebuild LMS App with DNS

cd ~/lms/webapp
vi .env


VITE_API_URL value to https://your-domain/api
 

npm run build
sudo rm -rf /var/www/html/*
sudo cp -r ~/lms/webapp/dist/* /var/www/html

 







1st Sep 2023 

Artifact Management DevOps
Artifact management is a crucial component of the DevOps process. It involves the management of software artifacts.
Artifact management helps in the automation of the build and release process, making it easier to deploy software updates and patches.

 






Binary Repository Manager


●	A Binary repository manager is a software tool designed to optimise the download and storage of binary files used and produced in software development.

●	It centralises the management of all the binary artifacts generated and used by the organization.

●	As part of the development lifecycle, source code is continuously being built into binary artifacts using Continuous Integration.

●	The Binary repository manager we are using is Nexus

 




 
Setting Up NEXUS

 


●	Nexus Requires “Standard_D2s_v3 size to work in AZURE, if you’re using AWS go with “t2.large instance”

●	Nexus works on “port 8081”, make sure to add port 8081 as part of your Security Group

●	Using Docker, Install Nexus

sudo ss -ntpl
sudo docker run -d -p 8081:8081 --name nexus sonatype/nexus3
sudo ss -ntpl

●	Browse the public-ip:8081
●	Default username is admin

●	Default Password can be checked with following command 

sudo docker container exec nexus cat /nexus-data/admin.password


zip lms-1.1.zip -r dist


curl -v -u username:password --upload-file <file> <nexus-repo-link>

Download Artifacts from Nexus Using following Command 
curl -u admin:Admin123* -X GET 'http://20.172.187.108:8081/repository/lms/lms-1.1.zip' --output lms-1.1.zip







4th Sep 2023 
DevOps Practice - Containerisation

The containerisation platform has become increasingly popular in recent years due to its ability to simplify application deployment and management.
To implement containerisation we are going to use “DOCKER”
With Docker, DevOps teams can package an application and its dependencies into a single container(box) that can be deployed across multiple environments, including development, testing, and production.

Monolithic Architecture

Monolithic == formed of a single large block of stone

Monolithic architecture is a software design pattern where the entire application is built as a single, indivisible unit. 
 

As a result, many developers have turned to more flexible architectures, such as microservices, that allow for more modular and scalable development. 







Microservices Architecture

Micro == small

Microservices Architecture is a software development approach that involves building small, independent services that work together to create a larger application. This architecture is highly scalable and allows for greater flexibility in development and deployment when you have applications grow in size and complexity. 
 

Micro services - Developed by - Developers 
Micro services - Deployed by - DevOps Engineers

Virtualisation vs Containerisation
Virtualisation and containerisation are two different ways of managing software applications. 

Virtualisation
Virtualisation involves creating a virtual version of a hardware platform, allowing multiple operating systems to run on a single machine.

 

Containerisation

Containerisation, on the other hand, is a newer technology that has gained popularity in recent years. 

Containerisation is lightweight and efficient, as it allows multiple applications to run on the same operating system, without the need for a complete virtual machine. This can be especially useful for running microservices.

 



 

Virtualization Implementation - AWS / AZURE / etc

Containerisation Implementation - Docker  / libvirt / etc


 
Container

 

 

 


 

 

In terms of software development, a container is an object for holding or transporting applications.

Docker

Docker is an open-source containerization platform(which helps you create containers) that allows developers to easily package, deploy, and run their applications in any environment.

 

 

Docker is especially useful for microservices architecture, 
With Docker, developers can build, ship, and run distributed applications easily and quickly, without worrying about the underlying infrastructure.
 



5th Sep 2023 
Docker Architecture
Docker architecture consists of the 
Docker daemon, the Docker client, and a Docker registry. 
The Daemon/Service is responsible for managing Docker objects such as images, containers, and networks. All the heavy lifting is done by daemon.
The client sends commands to the daemon and receives output. 
The registry stores Docker images and allows them to be shared among users and systems.
 
Docker Image
A Docker image is a lightweight, standalone, and executable package that includes everything needed to run the desired software application.
Docker Images are built from a Dockerfile, which is a script that contains all the commands to assemble the image.
 
Docker Container

A container in Docker is an isolated environment that allows you to run an application or service with all the dependencies it needs, without interfering with other applications or services running on the same system. To create a container we need Docker Image.

 

Setup Docker

●	We can install docker on any operating system whether it is Linux, Windows or MAC.

docker
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
docker


6th Sep 2023 
Detached/Background Mode
docker container run -dt nginx

The -dt flag indicates that the container should be started in detached mode, meaning that it will run in the background 

Port Forward / Mapping

 


 


















7th Sep 2023 


Data Persistency
 

●	By default containers are non-persistent in nature.

Docker Volumes
Docker Volumes are a feature in Docker that allow for data to be stored and shared between containers. 

Volumes provide a way to persist data generated by and used by Docker containers. One of the benefits of Docker Volumes is that they can be used to store data separately from the container itself. This means that even if a container is deleted, the data stored in the volume will remain.





Docker Volume Types

In Docker, there are three types of volumes that can be used to manage data persistency between containers and the host machine:

Named Volumes
Named volumes are explicitly created and given a user-defined name. They are managed by Docker, but the user can specify the name when creating the volume. Named volumes offer easy data management and can be shared across multiple containers. They are the recommended approach for most use cases.
Creating a named volume:

docker volume ls
docker volume create my_volume
docker volume ls

Using a named volume in container creation:

docker container run -dt --name my_container -v my_volume:/path/in/container my_image

You can use the "-v" flag to mount a volume from your host machine to the container. The syntax for this flag is "-v [host directory]:[container directory]". For example, in the command "docker container run -d --name my_container -v my_volume:/path/in/container my_image", the volume named "my_volume" is mounted to the container's "/path/in/container" directory.

By running the "docker container run" command with these parameters and flags, you can create a customised and fully functional Docker container that meets your specific needs and requirements.




Host Bind Mounts 
Host bind mounts allow you to mount a directory from the host system into a container. With bind mounts, changes in the container are immediately visible on the host and vice versa. This can be useful during development or when you want to share specific directories with the container.

Using a host bind mount in container creation:

docker container run -dt --name my_container -v /host/path:/path/in/container my_image

You can also specify a volume to be mounted in the container using the "-v" flag. In this example, we are mounting the directory "/host/path" on the host machine to the directory "/path/in/container" inside the container.

Anonymous Volumes
Anonymous volumes are automatically created and managed by Docker when you define a volume in the Dockerfile using the VOLUME instruction without specifying a name. Anonymous volumes are useful when you need temporary or throwaway storage within a container.

Defining an anonymous volume in Dockerfile:

FROM my_base_image
VOLUME /path/in/container





8th Sep 2023 
Dockerize Applications

●	Dockerizing an application is the process of converting an application to run within a Docker container. 

What Is a Dockerizing

●	Dockerizing is the process of packing, deploying, and running applications using Docker containers. Containers are created from images that specify their precise contents.

Docker Custom Images

●	Docker can build images automatically by reading the instructions from a Dockerfile.

●	A Dockerfile is a text document that contains all the commands a user could call on the command line to assemble an image.









●	Let us first start with the overall flow, which goes something like this:
○	You create a Dockerfile with the required instructions.
○	Then you will use the docker build command to create a Docker image based on the Dockerfile that you created
○	Then you can run the container using the image built

 
●	FROM — set base image
●	COPY — copy files to image
●	RUN — execute command in container
●	ENV — set environment variable
●	WORKDIR — set working directory
●	VOLUME — create mount-point for a volume
●	CMD — set executable for container











Dockerize Ecomm App

●	Make sure you have access to code
●	Make sure you know the manual procedure first
●	Update the manual procedure in Dockerfile with commands
●	Use docker build command to create docker image
●	Create a Docker Hub Account
●	Authenticate Docker Host with Docker Account
●	Test Docker Image by creating container
●	Push Docker Image To Docker Account























11th Sep 2023 

Dockerize LMS App
LMS App CODE

> git clone -b dev https://github.com/ravi2krishna/lms.git

IMPORTANT Fork Above Project to your Github Accounts

Perform Code Analysis on LMS App

Make sure to change the username here from ravi2krishna to your username

ls
git clone -b dev https://github.com/ravi2krishna/lms.git
ls
cd ~/lms/webapp









Dockerize LMS Backend - Process

git clone -b dev https://github.com/ravi2krishna/lms.git
cd ~/lms/api

vi .env

MODE=production
PORT=8080
DATABASE_URL=postgresql://postgres:Admin123*@db-container-ip:5432/postgres

vi Dockerfile

# FROM - Set Base Image
FROM node:16

# LABEL - add custom data, just some key values
LABEL maintainer="Backend API Maintainers <ravi2krishna@gmail.com>"

# ENV - Environment Variable
ENV APP_PATH /backend
ENV APP_VERSION 1.1

# RUN - execute commands
RUN mkdir $APP_PATH

# WORKDIR - working directory
WORKDIR $APP_PATH

# COPY - copy files to above image
COPY . .

# RUN - build related commands
RUN npm install
RUN npx prisma generate
RUN npm run build

# EXPOSE - Bind a port to container
EXPOSE 8080

# CMD - default program to start
CMD ["npm", "start"]

docker build -t ravi2krishna/9am-lms-be:prod .

docker container run -dt --name be -p 8080:8080 ravi2krishna/9am-lms-be:prod

Locally verify 
curl http://localhost:8080/api

{"message":"success","mode":"production"}

Verify with Browse - http://public-ip:8080/api
 




12th Sep 2023 

Multi Stage Builds

A multi-stage build process in Docker allows you to build a Docker image in multiple stages, where each stage focuses on a specific task.

In a multi-stage build, you define multiple FROM instructions in the Dockerfile, each representing a different build stage. Each stage has its own base image and set of instructions, and you can copy files or artifacts between stages using the COPY --from=<stage> instruction.


The multi-stage build process is particularly useful for compiled languages like C++, Java, or Node.js, where you need to build tools and dependencies during the compilation phase, but you don't want to include them in the final production image.












Dockerize LMS Frontend - Process

> vi Dockerfile

# FROM - Set Base Image
FROM node:16 AS builder

# LABEL - add custom data, just some key values
LABEL maintainer="Frontend API Maintainers <ravi2krishna@gmail.com>"

# ENV - Environment Variable
ENV APP_PATH /frontend

# RUN - execute commands
RUN mkdir $APP_PATH

# WORKDIR - working directory
WORKDIR $APP_PATH

# COPY - copy files to above image
COPY . .

# RUN - build realated commands
RUN npm install
RUN npm run build

# FROM - To Deploy
FROM nginx

# COPY - copy files to Nginx
COPY --from=builder /frontend/dist /usr/share/nginx/html


Docker Compose


 

Docker Compose


●	Compose is a tool for defining and running multi-container Docker applications. With Compose, you use a single YAML file to configure your application’s services(containers). Then, with a single command, you create and start all the services from your configuration.












13th Sep 2023 

High Availability

 

 

 



 











 















14th Sep 2023 

What is Kubernetes


 
Production-grade orchestration
Production-grade container orchestration refers to the capability of running containerized applications in a production environment effectively and reliably.

Several container orchestration platforms are considered production-grade, with Kubernetes being one of the most prominent and widely adopted solutions.


●	Kubernetes builds upon 15 years of experience of running production workloads at Google,


●	It was originally designed by Google, and is now maintained by the Cloud Native Computing Foundation(CNCF) .


 
Kubernetes Architecture
Master / Control Plane Components

API Server: 
The API server acts as the brain of the Kubernetes cluster. It provides a central point of communication for all the other components. When you want to create, update, or delete something in the cluster, you communicate with the API server.

Controller Manager: 
The Controller Manager is like the supervisor of the cluster. It continuously observes the state of the cluster through the API server. If it detects that the actual state of the cluster doesn't match the desired state (for example, if an app/container/pod goes down), it takes action to make the cluster converge to the desired state.
Scheduler: 
The Scheduler is like a matchmaker. Its job is to decide which worker node should run each new app/container/pod. It considers factors like available resources, to make sure app/container/pods are placed on suitable worker nodes.
etcd: 
Think of etcd as the memory of the Kubernetes cluster. It stores the configuration data and the state of the entire cluster. When any component wants to know the current state of the cluster, it asks etcd.

Worker Components

Kubelet: 
 The Kubelet is like the worker's Agent Software.  It runs on every worker node and is responsible for making sure that the containers/pods assigned to its node are running and healthy. It takes care of starting, stopping, and monitoring containers within the containers/pods. It updates the status back to Master.

Docker: 
The container runtime is the software that runs and manages containers.  The container runtime is responsible for pulling container images from a registry, creating containers, and managing their life cycles.


Kube Proxy: 
The Kube Proxy is like the traffic cop of the worker nodes. It manages the network connections and routing between the containers/pods and services within the cluster. It ensures that network traffic is correctly directed to the right destination.

In simple terms, the Kubernetes master components are the brain and the decision-makers of the cluster, while the worker components are the hands-on workers responsible for running and managing containers on each node. 

The master components take care of orchestrating and managing the entire cluster, ensuring that the desired state of the system matches the actual state. The worker components are responsible for running and maintaining the containers that make up the applications and services running in the cluster. Together, these components form the foundation of a robust and scalable container orchestration platform that makes it easier to deploy and manage applications in a distributed environment.








 

Setup Kubernetes

●	Now if you want to test something on your local environment or maybe try something very quickly on kubernetes, for example deploying a new application, 

●	Now obviously setting up a cluster like the above would be pretty difficult and not suitable if you don't have enough resources(cpu & memory) in the local machine.


Minikube
●	So basically minikube is a single node cluster, where the master processes and worker processes both run on one node, with docker runtime pre-installed 

 










15th Sep 2023 
Minikube

●	Minikube is a tool that allows developers and DevOps teams to run a single-node Kubernetes cluster on a local machine. It is primarily used for local development, testing, and learning purposes. 

●	Minikube implements a local Kubernetes cluster on macOS, Linux, and Windows. 

●	It's important to note that while Minikube is great for local development and testing, it is not designed for running production workloads at scale. 

 
Minikube Setup


Minikube Installation

●	Guide - https://minikube.sigs.k8s.io/docs/start/

●	Use t2.large instance with 20 GB EBS Volume and allow All Traffic. 

Setup Docker

docker
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
sudo usermod -aG docker ubuntu
logout
docker


Setup Minikube

minikube
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
minikube
minikube status
minikube start
minikube status


Kubectl

After starting Minikube, you can interact with the Kubernetes cluster using the kubectl command-line tool. 

kubectl is the primary command-line interface for interacting with Kubernetes clusters.


KUBECTL Setup

●	The Kubernetes command-line tool, kubectl, allows you to run commands against Kubernetes clusters. 

●	You can use kubectl to deploy applications, inspect and manage cluster resources, and view logs.
○	https://kubernetes.io/docs/tasks/tools/


kubectl
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x kubectl 
sudo mv kubectl /usr/local/bin/kubectl
kubectl







●	Important thing to note here is KUBECTL is not just for minikube, you can use it for any cluster.  


 








Kubernetes Objects Concepts

●	Making use of Kubernetes requires understanding the different abstractions it uses to represent the state of the system, such as pods, services, deployments etc. These are basically called kubernetes objects.

●	Kubernetes objects represent the state of your cluster 
○	These objects can be thought of as a sort of blueprint for the desired state of your application, and Kubernetes works tirelessly to ensure that the actual state of your cluster always matches this desired state. 
○	But objects in Kubernetes are not just static blueprints - they can be dynamically updated and modified as necessary, giving you the flexibility and agility you need to respond to changing business requirements and user needs.

●	By creating an object, you’re effectively telling the Kubernetes system what you want your cluster’s workload( what applications to run in the cluster) to look like, this is your cluster’s desired state.

●	Once you create the object, the Kubernetes system will constantly work to ensure that object(Applications) exists. 


●	To work with Kubernetes objects, whether to create, modify, or delete them, you’ll need to use a command-line tool called KUBECTL. 



Object Spec & Status

●	Every Kubernetes object includes two fields that govern the object’s configuration:
○	 the object spec (specification)
○	 the object status

The object spec, which you must provide, describes your desired state for the object(application), the characteristics that you want the object to have. 

●	For example run nginx application

 
One way to create an Object  like the one above, we use the kubectl apply command, passing the .yaml file as an argument.

●	The object status describes the actual state of the object, and is supplied and updated by the Kubernetes system.

●	At any given time, the Kubernetes actively manages an object’s actual state to match the desired state you supplied. 






Pod Object

●	A Pod is the basic execution unit inside kubernetes or the basic building block inside kubernetes is POD.

●	A Pod represents a unit of deployment: a single instance of an application in Kubernetes. 

 




Manage Objects

●	Manage Objects inside kubernetes can be done using
○	Commands - Imperative Commands
○	CODE - Declarative Configuration files or Manifests



19th Sep 2023 



Pod Issues

It's important to note that creating pods directly using `kubectl run` is not the recommended way to manage applications in Kubernetes for production use. For long-term or more complex deployments, it's better to use higher-level abstractions like Deployments, which provide additional features like scaling, rolling updates, and self-healing. Deployments help manage the desired state of pods and offer more control over the application lifecycle in Kubernetes.



●	Warning - It is recommended that users create Pods only through a Controller(Deployments) and not directly. 

●	PODS are ephemeral in nature i.e they can DIE/DISPOSABLE.




 





kubectl get pods
kubectl delete pod nginx-pod
kubectl get pods

Declarative Configuration Files
Pod Spec

https://kubernetes.io/docs/concepts/workloads/pods/

> vi nginx-pod.yml

apiVersion: v1
kind: Pod
metadata:
  name: nginx-pod
spec:
  containers:
  - name: nginx-container
    image: nginx
    ports:
    - containerPort: 80


kubectl get pods
kubectl apply -f nginx-pod.yml
kubectl get pods

ReplicaSet Object

●	Replica Set is one of the key features of Kubernetes, which is responsible for managing the pod lifecycle. 


●	Replica Set Object is responsible for making sure that the specified number of pod replicas are running at any point of time. As such, it is often used to guarantee the availability of a specified number of pods.


 










●	It is better to use the Replica Set to manage the pod life cycle rather than creating a pod again and again.

●	https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/


20th Sep 2023 

Replicaset Issues

●	Warning: In many cases it is recommended to create a Deployment instead of ReplicaSet.


●	What replicasets don’t allow are updates. If a newer version of your app, say, app:v2 comes along, you have to delete the existing replicaset and create a new one. This is where the concept of deployments comes in handy.









Deployment Object

●	A deployment provides updates for pods and replica sets.

 

 






Service Object

●	A service is an endpoint, which you use to access the pods.

●	So when you create a pod, you cannot expose pods directly to the world, for this to happen we need a service object. 

●	https://kubernetes.io/docs/concepts/services-networking/service/



●	There are different types of kubernetes services present
○	ClusterIP
○	NodePort
○	LoadBalancer
○	ExternalName


●	The type property in the Service's spec determines how the service is exposed to the network.

ClusterIP Service

●	ClusterIP is the default and most common service type.

●	Kubernetes will assign a cluster-internal IP address to ClusterIP service. This makes the service only reachable within(intranet or local) the cluster.

●	You cannot make requests to service (pods) from outside the cluster.


Use Cases

●	Inter service communication within the cluster. For example, communication between your database and api.

 

 














Postgres Deployment 

> cat lms-posgtres-deployment.yml

apiVersion: apps/v1
kind: Deployment
metadata:
  name: postgres-deployment
  labels:
    tier: db
spec:
  replicas: 1
  selector:
    matchLabels:
      tier: db
  template:
    metadata:
      labels:
        tier: db
    spec:
      containers:
      - name: postgres
        image: postgres
        ports:
        - containerPort: 5432
        env:
        - name: POSTGRES_PASSWORD
          value: Admin123*






Postgres Service

> cat lms-postgres-svc.yml

apiVersion: v1
kind: Service
metadata:
  name: postgres-service
spec:
  type: ClusterIP
  ports:
  - port: 5432
  selector:
    tier: db


> kubectl run postgresql-postgresql-client --rm --tty -i --restart='Never' --namespace default --image bitnami/postgresql --env="PGPASSWORD=<HERE_YOUR_PASSWORD>" --command -- psql --host <HERE_HOSTNAME=SVC_NAME_OR_IP> -U <HERE_USERNAME> 











21st Sep 2023 

NodePort Service

●	NodePort exposes the service on each Node’s IP at a static port (the NodePort). Each node proxies that port into your Service. So, external traffic has access to a fixed port on each Node. 


●	You can contact the NodePort Service, from outside the cluster, by requesting <NodeIP>:<NodePort>.

●	Node port must be in the range of 30000–32767. Manually allocating a port to the service is optional. If it is undefined, Kubernetes will automatically assign one.

●	If you are going to choose a node port explicitly, ensure that the port was not already used by another service.

Use Cases

●	When you want to enable external connectivity to your service.

Warning : 
●	Prefer to place a load balancer above your nodes to avoid node failure.






 











Secrets

A Secret is an object that contains a small amount of sensitive data such as a password, a token, or a key. Such information might otherwise be put in a Pod specification or in a container image. Using a Secret means that you don't need to include confidential data in your application code.

Because Secrets can be created independently of the Pods that use them, there is less risk of the Secret (and its data) being exposed during the workflow of creating, viewing, and editing Pods


ConfigMaps

A ConfigMap is an API object used to store non-confidential data in key-value pairs. Pods can consume ConfigMaps as environment variables, command-line arguments, or as configuration files.

A ConfigMap allows you to decouple environment-specific configuration from your container images, so that your applications are easily portable.

Caution: ConfigMap does not provide secrecy or encryption. If the data you want to store are confidential, use a Secret rather than a ConfigMap, or use additional (third party) tools to keep your data private.





>  kubectl exec -i -t pod/pod-name --container container-name -- command


25th Sep 2023 

Kubernetes Production Setup

 

In production environments, it is common to use managed Kubernetes services provided by cloud providers rather than running and managing your own Kubernetes clusters.



High Availability and Reliability: Managed Kubernetes services are designed to provide high availability and reliability. They typically run multiple master nodes across different availability zones, ensuring that the control plane is resilient to failures. They also manage the underlying infrastructure to maintain a stable environment.

Popular examples of managed Kubernetes services include Amazon Elastic Kubernetes Service (Amazon EKS) on AWS, Azure Kubernetes Service (AKS) on Microsoft Azure, and Google Kubernetes Engine (GKE) on Google Cloud Platform.


EKS Setup
●	Use IAM( Identity & Access Management ) Service to create a account for eks(username : eks-user)

> Create an IAM User > eks-user > Apply AdministratorAccess Policy To  eks-user > Enable Console Access - Access & Secret Keys as well.

 
> open the IAM service, click Users, select the user. On the Permissions tab click the Add Inline Policy link.





The following policy adds all permissions to the user.

{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "eksadministrator",
            "Effect": "Allow",
            "Action": "eks:*",
            "Resource": "*"
        }
    ]
}

 

Switch to IAM User

> Make sure to login into console with eks-user then perform the next steps 


 

 

> Create an IAM Role > Scroll Down > Select EKS > Select EKS Cluster > Next Permissions > Select : AmazonEKSClusterPolicy > Next > Review > Role Name : MyEKSRole > Create 

> AWS Services > EKS > Clusters > Create Cluster > Name : myeks > Kubernetes Version : 1.24 > Cluster Service Role : MyEKSRole > Next > VPC : Select Default VPC > Subnets : Keep Defaults > Security Groups : leave as it is > Choose cluster ip address family : IPv4 > Cluster endpoint access : Keep Public & Private > Next > Configure logging : keep all defaults > Next > Amazon EKS Add-ons : Keep Defaults > Next > Next > Create Cluster (15 mins)

NodeGroup Creation

●	Let's now create Worker Nodes

 

●	Create IAM Role with following policies 
○	AmazonEKSWorkerNodePolicy
○	AmazonEKS_CNI_Policy
○	AmazonEC2ContainerRegistryReadOnly

●	AWS > Services > IAM > Roles > Create Role > Select AWS Service > Use Case : EC2 > Policy : AmazonEKSWorkerNodePolicy - AmazonEKS_CNI_Policy - AmazonEC2ContainerRegistryReadOnly  > Next > Role Name : AppName-EKSWorkerNodeRole > Create Role

●	Goto EKS Cluster > Compute > Node Group > Add Node Group > AppName-NodeGroup > NodeIAM Role > Role : AppName-EKSWorkerNodeRole > Next > Select t3.medium Instance Type (faster) > Disk EBS : 20 GB > Desired : 2 > Minimum :2 > Maximum 5 > Next > Node group nw configuration : select all four subnets > Next > Next > Create 



26th Sep 2023 
Client Machine Creation
Setup Docker

docker
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
sudo usermod -aG docker ubuntu
logout
docker

Setup KUBECTL

●	> kubectl 
●	> curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.23.6/bin/linux/amd64/kubectl
●	> chmod +x kubectl
●	> sudo mv kubectl /usr/local/bin/kubectl
●	> kubectl 






Setup AWS CLI

●	> aws
●	> curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
●	> sudo apt -y install unzip
●	> unzip awscliv2.zip
●	> sudo ./aws/install
●	> aws

Load Balancer Service
Exposes the Service externally using an external load balancer. Kubernetes does not directly offer a load balancing component; you must provide one, or you can integrate your Kubernetes cluster with a cloud provider(AWS).

 









27th Sep 2023 

> cat nginx-loadBalancer-svc.yml
apiVersion: v1
kind: Service
metadata:
  name: nginx-service
spec:
  type: LoadBalancer
  ports:
  - port: 80
  selector:
    tier: frontend

> kubectl apply -f nginx-loadBalancer-svc.yml


Postgres Deployment 

> cat lms-posgtres-deployment.yml

apiVersion: apps/v1
kind: Deployment
metadata:
  name: postgres-deployment
  labels:
    tier: db
spec:
  replicas: 1
  selector:
    matchLabels:
      tier: db
  template:
    metadata:
      labels:
        tier: db
    spec:
      containers:
      - name: postgres
        image: postgres
        ports:
        - containerPort: 5432
        env:
        - name: POSTGRES_PASSWORD
          value: Admin123*






Postgres Service

> cat lms-postgres-svc.yml

apiVersion: v1
kind: Service
metadata:
  name: postgres-service
spec:
  type: ClusterIP
  ports:
  - port: 5432
  selector:
    tier: db

> kubectl run postgresql-postgresql-client --rm --tty -i --restart='Never' --namespace default --image bitnami/postgresql --env="PGPASSWORD=<HERE_YOUR_PASSWORD>" --command -- psql --host <HERE_HOSTNAME=SVC_NAME_OR_IP> -U <HERE_USERNAME> 


Image Preparation

git clone -b dev https://github.com/ravi2krishna/lms.git
cd lms/api

vi .env

MODE=production
PORT=8080
DATABASE_URL=postgresql://postgres:Admin123*@postgres-service:5432/postgres

vi Dockerfile

# FROM - Set Base Image
FROM node:16

# LABEL - add custom data, just some key values
LABEL maintainer="Backend API Maintainers <ravi2krishna@gmail.com>"

# ENV - Environment Variable
ENV APP_PATH /backend
ENV APP_VERSION 1.1

# RUN - execute commands
RUN mkdir $APP_PATH

# WORKDIR - working directory
WORKDIR $APP_PATH

# COPY - copy files to above image
COPY . .

# RUN - build related commands
RUN npm install
RUN npx prisma generate
RUN npm run build

# EXPOSE - Bind a port to container
EXPOSE 8080

# CMD - default program to start
CMD ["npm", "start"]

docker build -t ravi2krishna/9am-lms-be .
docker login -u ravi2krishna
docker push ravi2krishna/9am-lms-be





Backend / API Deployment 

> cat lms-api-deployment.yml

apiVersion: apps/v1
kind: Deployment
metadata:
  name: api-deployment
  labels:
    tier: backend
spec:
  replicas: 1
  selector:
    matchLabels:
      tier: backend
  template:
    metadata:
      labels:
        tier: backend
    spec:
      containers:
      - name: api
        image: ravi2krishna/9am-lms-be
        ports:
        - containerPort: 8080









Backend / API Service

> cat lms-api-svc.yml

apiVersion: v1
kind: Service
metadata:
  name: api-service
spec:
  type: LoadBalancer
  ports:
  - port: 8080
  selector:
    tier: backend



Frontend Deployment 

> cat lms-frontend-deployment.yml

apiVersion: apps/v1
kind: Deployment
metadata:
  name: frontend-deployment
  labels:
    tier: frontend
spec:
  replicas: 1
  selector:
    matchLabels:
      tier: frontend
  template:
    metadata:
      labels:
        tier: frontend
    spec:
      containers:
      - name: frontend
        image: ravi2krishna/9am-lms-fe
        ports:
        - containerPort: 80






Frontend Service

> cat lms-frontend-svc.yml

apiVersion: v1
kind: Service
metadata:
  name: frontend-service
spec:
  type: LoadBalancer
  ports:
  - port: 80
  selector:
    tier: frontend






19th Oct 2023 

Terraform

Infrastructure As Code - IaC

●	Infrastructure as code is the process of managing and provisioning computer data centers through machine-readable definition files [CODE].


 

●	Like Developers write Application Code to build Applications
○	Technologies - Java, Python, Node etc

●	As a DevOps Engineer will be writing Infrastructure Code to build Infrastructure
○	Tools - AWS Cloudformation, Azure ARM, Terraform etc

Terraform

●	Terraform is an Infrastructure As Code [IaC] software from HashiCorp. 

 
●	Infrastructure is defined in HCL [Hashicorp Configuration Language]
Terraform Setup & Tools

●	Setup Terraform Workstation (AWS/AZURE) 
●	Install Git (To Track Code)
●	Install AWS CLI (to authenticate AWS Account)
●	Install AZURE CLI (to authenticate AZURE Account)
●	Install Terraform


Installations

aws
az
sudo apt update -y
sudo apt  install awscli -y
sudo apt install azure-cli -y
aws
az
terraform
# https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli
terraform


Terraform is an infrastructure as code tool that enables you to safely and predictably provision and manage infrastructure in any cloud.






 

AWS - AZURE Providers

●	AWS, Azure etc 
○	 https://registry.terraform.io/providers/hashicorp/aws/latest/docs
○	https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs








20th Oct 2023 

IaC Benefits

●	IaC boosts productivity through automation

●	Consistency in Setup & Configuration

●	Minimising risk of human errors

●	Replicate your infrastructure easily, CODE = REUSABILITY

●	Makes your infrastructure Auditable, Since you can version control IaC configuration files like any source code file, you have full traceability of the changes



AWS Provider

●	Use the Amazon Web Services (AWS) provider to interact with the many resources supported by AWS. 

●	You must configure the provider with the proper credentials before you can use it.

 
AWS IAM 
With AWS Identity and Access Management (IAM), you can specify who or what (terraform) can access services and resources in AWS.

●	AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources. 

●	You use IAM to control who is authenticated (signed in) and authorised (has permissions) to use resources.

 
Terraform says, you must configure the provider with the proper credentials before you can use it.

 

> AWS > IAM > Users > Create User (terraform) > Apply Administrator Access Policy > Create User

 

> Select terraform user > Security Credentials tab > Access Keys > Create Access Keys > Select Command Line Interface > Create

> Download .csv file which contains the credentials 
Terraform Resources

●	Resources are the most important element in the Terraform language. Each resource block describes one or more infrastructure objects, such as virtual networks, compute instances, or higher-level components such as DNS records.
●	Use resource blocks to define components of your infrastructure. 
●	A resource might be an Subnet, Security Group, EC2 instance etc
●	Resource blocks have two strings before the block: the resource type and the resource name. 
●	Together, the resource type and resource name form a unique ID for the resource.
●	Resource blocks contain arguments which you use to configure the resource. Arguments can include things like machine sizes, disk image names, or VPC IDs.
●	Check the Provider Resource Document Always 
○	https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group

○	https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ebs_volume

 

Initialize Terraform

●	When you create a new configuration — or check out an existing configuration from version control — you need to initialize the directory with terraform init.
●	Initialising a configuration directory downloads and installs the providers defined in the configuration, which in this case is the aws provider
●	Terraform downloads the aws provider and installs it in a hidden subdirectory of your current working directory, named .terraform.
●	Terraform also creates a lock file named .terraform.lock.hcl which specifies the exact provider versions used, so that you can control when you want to update the providers used for your project.
	
	> terraform init

Provisioning Infrastructure

●	Terraform's primary function is to create, modify, and destroy infrastructure resources to match the desired state described in a Terraform configuration.

●	When people refer to "running terraform," they generally mean performing these provisioning actions in order to affect real infrastructure objects. 

●	Terraform's provisioning workflow relies on three commands: 
○	plan, apply, and destroy. 
○	All of these commands require an initialized working directory, and all of them act only upon the currently selected workspace.

Terraform AWS Code

https://github.com/ravi2krishna/tf-9-1030-am/tree/aws


Terraform AZURE Code

https://github.com/ravi2krishna/tf-9-1030-am/tree/azure







<!---
dbjkerhfiu/dbjkerhfiu is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
