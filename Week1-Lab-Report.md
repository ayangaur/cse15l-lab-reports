# Remote Access
 
## Step 1: Installing Visual Studio Code

To install VS Code, go to the website, [Visual Studio Code](https://code.visualstudio.com/). Over here you will find instructions on how to download VS Code for all Operating  Systems.

Once it has been installed open VS Code and you should see a window like this,

<img width="1024" alt="Screenshot 2023-01-11 at 4 05 47 PM" src="https://user-images.githubusercontent.com/122495485/211944504-6712f8d4-97ba-4af3-bbd3-da54ae829c4b.png">
  
## Step 2: Remote Connection

If you are on Windows you must first download 'git' for Windows. You can use this website to downlaod git, [Git for Windows](https://gitforwindows.org/). Now you must set your default terminal to 'git bash'. You can follow this tutorial to do so,
[Git Bash on Windows](https://stackoverflow.com/a/50527994).
Now you can go ahead and create a new terminal by clicking on Terminal and then New Terminal in the Toolbar.

<img width="280" alt="Screenshot 2023-01-11 at 4 42 31 PM" src="https://user-images.githubusercontent.com/122495485/211948892-8ef8f241-c79f-44cc-9e9d-81cbdcb94258.png">

Using your CSE15L course specific account you can start connecting by running the following command,

`$ ssh your-username@ieng6.ucsd.edu`
    
If this is the first time you're connectiing to this server you will be prompted with the following,
  
```
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```

You can answer 'yes' to this question, after which you will be asked to enter your password. Enter the password you set for your CSE15L account, after which you should see the following,

<img width="519" alt="Screenshot 2023-01-11 at 4 27 21 PM" src="https://user-images.githubusercontent.com/122495485/211947152-f14dd025-1d5b-4c4e-bbb4-0d445420f144.png">

You are now connected to the device.

## Step 3: Trying Commands

We can now start trying commands such as `cd`, `ls`, `pwd`, `cp`, and `cat`.
These commands will give you various outputs. If you try to access files from stored on your local computer, you will not be able to do so.
The above mentioned commands have the following meanings:
- `cd`: Change Directory (The path of the new directory needs to be provided)
- `ls`: Lists the files in current directory, the format the files are dispayed in can be changed using `ls -lat` or `ls -a`
- `pwd`: Shows your current directory
- `cp`: Copies the mentioned file to the mentioned directory
- `cat`: Prints out the text in your file.

<img width="768" alt="Screenshot 2023-01-11 at 3 54 18 PM" src="https://user-images.githubusercontent.com/122495485/211947809-0fde545d-565c-4f81-8811-f2c40015c80e.png">

The commands should show you something similar. There are various more commands you can use, and you can start accessing and editing files on the remote server.

If you are done using the server you can log out using:
- Ctrl+D
- Running the command `exit`
