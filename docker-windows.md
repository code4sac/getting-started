# Getting Started with CodeForSacramento Projects (Windows, VS Code)
## Prerequisites
1. [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/install)<br>
2. [Docker for Windows](https://www.docker.com/products/docker-desktop/)

## Setting up the WSL environment

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

** Note: it is important to clone any projects into the ~/ path inside of WSL, and not clone projects into a normal windows path.
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
 
If you have made it this far, you have successfully setup docker and it is working properly.  However, you may need the following additional steps to setup git.
 
Check if you have an existing SSH key, and if you know the password to it

`ssh-keygen -y -f ~/.ssh/id_rsa | less`

If you see were able to see the key, press q and skip the Generate an SSH Key steps below.

## Generate an SSH Key

1. Move any existing keys if there are any

`mv ~/.ssh/id_rsa ~/.ssh/id_rsa.bak`
`mv ~/.ssh/id_rsa.pub ~/.ssh/id_rsa.pub.bak`

2. Follow the [Github Guide for generating a new SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=linux)



## Setup Git

1. Follow the [Github Guide for Adding a new SSH key to your Github account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
2. `git config --global user.email "you@example.com"`
3. `git config --global user.name "Your Name"`

Hopefully, by this line, you should be good to go 😀

