# Lab Report 1
This is a list of instructions on how to 1)Install VScode 2)Remotely Conntect and 3)Try commands in this remotely connected enviroment.

## Step 1: Installing VScode
If you already have VScode installed you do not need to reinstall it. 
Go to the [VScode website](https://code.visualstudio.com) and read/follow the instructions on the website to download the application. Make sure to keep in mind the OS you are running, for example macOS vs Windows vs Linux. 

After installation the window should look like this (however it may look slightly different depending on visual options. Ex: light vs. dark mode).
![Image](https://github.com/WillDiego/cse15l-lab-reports/blob/main/Screenshot%202023-04-05%20at%204.33.35%20PM.png)

## Step 2: Remote Connect
Go [here](https://sdacs.ucsd.edu/~icc/index.php) and follow the instructions on resetting your password. 
If you are using a windows device then dowload [git](https://gitforwindows.org) and navigate to [stackoverflow](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994) to learn about using bash on windows.
After this, open VScode again and create a new terminal window. In the terminal type '$ ssh cs15sp23AAzz@ieng6.ucsd.edu.' Where AA is replaced by the two letters accociated with your course account, this is found after logging into your account above before resetting your password. Then the terminal will prompt you for your newly reset password.
If its your first time connection to the server you will most likely be prompted with the following text
>⤇ ssh cs15lsp23zz@ieng6.ucsd.edu
>The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
>RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
>Are you sure you want to continue connecting (yes/no/[fingerprint])? 
ringringr
