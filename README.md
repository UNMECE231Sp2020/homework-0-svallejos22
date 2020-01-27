# Homework0
Homework 0 of ECE 231: Intermediate Programming. Assigned 1/24/2020. Due 1/31/2020, 11:59 pm.
The goal for this homework is the get acquainted with the software that you are going to be using for the rest of the semester. By the end of this assignment you will achieve two things:

    Get a Linux system working
    Create a GitHub account & have Git working on your linux system
  
  
## Getting a Linux system
There are few ways of doing this:
### Linux
If you have a Linux machine (Ubuntu, Pop!OS, Redhat, Linux Mint, etc), please take a look at setting up your Github account and getting Git working on your machine.
### All operating systems (except Linux)
You can download a virtual machine that can host a different operating system. I like to use VM Virtual Box (because its free) and the link to download the software is here:

[VM Virtual Box](https://www.virtualbox.org/wiki/Downloads)

Once you have downloaded Virtual Box feel free to download your favorite Linux OS, for first timers I recommend Ubuntu:
[Ubuntu OS](https://ubuntu.com/download)

Some notes about the configuration of the VM, please allocate (if possible) about 20 GB of storage space (at minimum 10 GB), and dedicate half or a quarter of your RAM to the VM.
### MacOS
You either can download Virtual Box from the section above or download Xcode to run C/C++ software. If you download Xcode you will be programming in your MacOS terminal.

### Windows
You either can dowload Virtual Box from the section above or activate and use the Linux system for Windows 10. You can follow the tutorial [here](https://www.maketecheasier.com/install-linux-subsystem-for-windows10/)

## Updating and downloading packages for your terminal
(If you have MacOS skip this step)
Once you have set up your Linux (not MacOS) system and have your terminal up and running type the following commands:

        sudo apt-get update -y
        sudo apt-get upgrade -y
        sudo apt-get dist-upgrade -y

This should update all current packages installed (and is needed before installing additional packages). After all the packages have been updated, type these commands:

        sudo apt-get install vim
        sudo apt-get install gcc
        sudo apt-get install make
        sudo apt-get install git

## Using git and github
[Here](https://www.youtube.com/watch?v=w3jLJU7DT5E) is a quick video on what github is. Please create an account on [github](https://github.com/) and create a new repository. WHEN YOU SIGN UP FOR GITHUB, PLEASE DO NOT USE YOUR UNM EMAIL, YOU WANT THIS ACCOUNT TO EXIST AFTER YOU GRADUATE. The idea is that you KEEP ADDING CODE THROUGHOUT YOUR CAREER AS A PROGRAMMER. Feel free to name your new repository anything you want (please keep it appropriate). Also, initialize your git repo with a README.md. You will be writing things like what kind of code the git repo has, what does the code do, how to use the code, etc..., to your README file. 

All your github repositories (git repos) will be public, as potential employers can see the code that you have created. This will show that you can work in groups and your git repos will be the proof.

Once you have created your git repo in github, open a terminal and type:
    
        git clone https://github.com/<github username>/<git repo name>
        cd <git repo name>

Where \<github username\> is your github username and \<git repo name\> is the name of the git repo that you have just created. After this is done, type:

        vim hello.cpp
        
Write a simple hello world program and add it to your git with this command:

        git add hello.cpp
        
(optional) you may type

        git status
        
And may find that git is keeping track of executables such as a.out, and other files, you can create a .gitignore (a hidden file), this file will tell git to not keep track of these files. You can create one that will not keep track of a.out this command:

        vim .gitignore
        
Inside of the file it should look like this:
        
        .gitignore
        a.out
        
Notice how I also added .gitignore, that is because .gitignore will not ignore itself.
(end optional)

Now that you have added a program to your git and added it, you need to write a commit that documents what you have done. Here is an example:

        git commit -m "Added a program called hello.cpp that prints Hello world!"
        
The only that should vary between git commits is what is between the double quotes. Please make your git commits meaningful. Not only will I be taking a look at your git commits, but fellow students as well (AND POTENTIALLY RECRUITERS). Lastly, type this command to upload changes to your git repo:

        git push
        
You will be asked to enter your github username and password and BAM! you will have updated your repo, type this command to see your history of commits:
    
        git log
        
Once you have created your git repo and added hello.cpp and updated your git repo (your repo should have two commits), you are done! 
## Optional downloads
To save some time in the second half of the course, if you have decided on what track you want to do for the second half of the course please download the environment needed.
### Anaconda Python distribution
[Anaconda IDE](https://www.anaconda.com/distribution/). I recommend using Spyder, but feel free to try the jupyter notebook. You can optionally download kite when you launch Spyder.
### Unreal Engine
You can dowload the Unreal Engine [here](https://www.unrealengine.com/). You will need to create an Epic Games store account to use the Unreal Engine and about 30 GB of storage space.
