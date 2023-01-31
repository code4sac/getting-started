<<<<<<< main
# Getting Started with CodeForSacramento Projects (Windows, VS Code)
Prerequisites<br>
1. [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/install)<br>
2. [Docker for Windows](https://www.docker.com/products/docker-desktop/)

When you are done installing WSL, and Docker, open WSL. Make sure that you are running WSL2, by using opening your Command Prompt terminal and typing this command: 

```wsl -l -v```

This is what you should be seeing: 

 <img src="https://i.imgur.com/7m1phu9.jpg"/>

Upon confirming that the correct version of Ubuntu is installed, open Microsoft Windows Subsystem (WSL). 

[Here are the instructions for WSL if/when you run into a problem.](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

Open WSL.<br>
Type the following commands (without the parenthesis and their content, explanations): 
1. ```cd ~``` (this command  is a shortcut that represents the user's home directory. This command is equivalent to running "cd" without any arguments).
2. ```cd codeForSac/``` (takes you to the CodeForSac folder).
3. ```code .```

The finished product should look something like this: 

<img src="https://i.imgur.com/3HVQBPX.jpg"/>

At this point, make sure that the Docker is running in the background, and VS Code is up and running. 

Depending on the project you are working on, make sure you cd to the right folder: 

For example, for the trash-ai project cd trash-ai, ```cd trash-ai```
When you re in the right folder, run the following command: ```make local```

Example: 

 <img src="https://i.imgur.com/W6364j4.jpg"/>
 
 This may take a minute or two. 
 
 When it's completed, open a separate terminal. Again, cd into the folder of choice. For the trash-ai, ```cd trash-ai/```
 
**Before you move to the next step, make sure that you have an SSH key, and you know your “passphrase”.** 

First thing you want to do is to check whether any changes to the code will be fetched or pushed to the right repository on GitHub. 
1. ```git remote -v```
2. If the repo is “codeForSac”, it needs to be changed to yours.  
3. To do that, you’d need an **SSH key**.
4. The SSH code below is for reference only, it’s an example of what would you see if you didn’t have an SSH key

![image](https://user-images.githubusercontent.com/97710680/214155615-8cb12e65-f734-4746-8bef-d7d4585d580d.png)

To create an SSH key, you’d have to type the following command: 
```cat ~/.ssh/if_rsa.pub```

And it should look like this:

![image](https://user-images.githubusercontent.com/97710680/214155858-0538c195-d3bd-45aa-8b73-89441737b000.png)

![image](https://user-images.githubusercontent.com/97710680/214155923-1c01bb4b-ccc3-4c81-8a8e-f072fedfe37b.png)

Next step is to check out the “git pull origin production”.

If it looks okay, meaning that changes are going to be implemented to your GitHub repo, go ahead and create a branch: ```git checkout -b deleteAbout``` (to make changes to that branch instead of the main repo).

You may be asked about get asked about your GitHub email and name, whatever name and email you used to sign up with GitHut 

![image](https://user-images.githubusercontent.com/97710680/214156202-a71dc02b-55c4-420a-90fa-7c1c7d2ddfda.png)

Hopefully, by this line, you should be good to go 😀



=======
# Getting Started
This repo for getting started contributing to Code for Sacramento


## Local Development
A lot of our repositories use Docker for local development.  Docker is a piece of software that allows us to package a lot of dependencies from the operating system level up into each project.  This means that you do not need to install many dependencies on your host system in order to run the majority of our active projects.

If you do not have docker installed, please do the following depending on your type of system:

- [Docker Windows](docker-windows.md)
- [Docker MacOS](docker-macos.md)


## Git
We use git for all of our projects, and it is necessary in order to contribute to our project code.  Below are some resources to get started with git.

- [Install Git Windows](git-windows.md)
- [Install Git MacOS](git-macos.md)
>>>>>>> main

