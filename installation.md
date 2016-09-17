## What you will learn in this section

This section will help you understand and install Python, git and django on your machine.
> Linux: Ubuntu, Linux Mint or any Debian based distro

> MacOS: Any version

> Windows: Windows 7, 8 or 10

> Don't type "$" in terminal

## Python Installation
Python 3 is released long back but due to industry adoption and available library in Python 2.7, in this course we will discuss only discuss about Python 2.7.xx. However, We have a defined roadmap for Python 3.x in coming days.

### Installation on Linux
Linux comes with Python installed so no need to install python. At Nescode, we use Linux Mint 17.3 LTS Edition.
Check the python version by below command:

```
$ python --version
Python 2.7.6
```

### Installation on OS X
OS X comes with python installed so no need to install python. Check the python version by below command:

```
$ python --version
Python 2.7.6
```

### Installation on Windows
Visit (https://www.python.org/downloads/) and download python 2.7.xx(At the time of writing this tutorial, it is Python 2.7.12). The installation is just like any other windows installer. It is important to remember the path (the directory) where you installed Python. It will be needed later!

One thing to watch out for: on the second screen of the installation wizard, marked "Customize", make sure you scroll down to the "Add python.exe to the Path" option and select "Will be installed on local hard drive", as shown here:

![Python path in windows](https://s3.amazonaws.com/nescodehellodjango/tutorial/msi_install_path.png)

To check python installation, open command prompt by pressing Windows+R, type in cmd, and hit enter. Type below command to check version:

```
C:\>_ python --version
Python 2.7.6
```

## Git installation
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. And git was created by Linus Torvalds - The founder of linux kernel in 2005 for development of the Linux kernel.

Using git, you can do incremental development in team. Git allows and encourages you to have multiple local branches that can be entirely independent of each other like:
- development
- master

### Get started
Getting started with git is very simple, you can setup git on Linux, MacOX and Windows machine within five minute.

### Linux setup

#### Step 1: Install git
Run below command to install git in terminal, it will install through binary-package management tools which comes by default in linux.
```
$ sudo apt-get install git
```
#### Step 2: Create GitHub account
Create a GitHub account at https://github.com/. GitHub is a web-based Git repository hosting service which will allow you publish and collaborate on code with other.

#### Step 3: Generate SSH Key and add it to GitHub account
SSH keys are a way to identify trusted computers without involving passwords. You can generate an SSH key and add the public key to your GitHub account by following the commands in same order:
```
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com" # Don't add any passphrase.
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_rsa
$ sudo apt-get install xclip
$ xclip -sel clip < ~/.ssh/id_rsa.pub
```
In the top right corner of page, click your profile photo, then click Settings. In sidebar, go to SSH and GPG Keys. Click new SSH Key and add your SSH Key which you have just now copied in clipboard. (Give a title to key and press Ctrl + V)

#### Step 4: Testing SSH Connection
After you've set up your SSH key and added it to your GitHub account, you can test your connection. Open your terminal and test
```
$ ssh -T git@github.com
```
### MacOS setup
Process of setting up git in Mac is same as Linux.

### Windows setup

#### Step 1: Install git
Just go to http://git-scm.com/download/win and the download will start automatically. Start installation setup by double clicking on .exe file. While installation, choose below options:
- In the fifth step entitled "Adjusting your PATH environment", choose "Use Git and optional Unix tools from the Windows Command Prompt" (the bottom option)
- Checkout Windows-style, commit Unix-style line endings is good.
Other than this, the defaults are fine.

#### Step 2: Create GitHub account
Create a GitHub account at https://github.com/. GitHub is a web-based Git repository hosting service which will allow you publish and collaborate on code with other.

#### Step 3: Generate SSH Key and add it to GitHub account
SSH keys are a way to identify trusted computers without involving passwords. You can generate an SSH key and add the public key to your GitHub account by following the commands in same order.

Note: Use Git Bash to perform execute below command, NOT windows command prompt.
```
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com" # Don't add any passphrase.
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_rsa
$ clip < ~/.ssh/id_rsa.pub
```
In the top right corner of page, click your profile photo, then click Settings. In sidebar, go to SSH and GPG Keys. Click new SSH Key and add your SSH Key which you have just now copied in clipboard. (Give a title to key and press Ctrl + V)

#### Step 4: Testing SSH Connection
After you've set up your SSH key and added it to your GitHub account, you can test your connection. Open your terminal and test
```
$ ssh -T git@github.com
```
