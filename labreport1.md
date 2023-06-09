# Lab Report 1
This is a list of instructions on how to 1)Install VScode 2)Remotely Conntect and 3)Try commands in this remotely connected enviroment.

## Step 1: Installing VScode
If you already have VScode installed you do not need to reinstall it. 

Go to the [VScode website](https://code.visualstudio.com) and read/follow the instructions on the website to download the application. Make sure to keep in mind the OS you are running, for example macOS vs Windows vs Linux. 

After installation the window should look like this (however it may look slightly different depending on visual options. Ex: light vs. dark mode).
![Image](https://github.com/WillDiego/cse15l-lab-reports/blob/main/scr3.png)

## Step 2: Remote Connect
Go [here](https://sdacs.ucsd.edu/~icc/index.php) and follow the instructions on resetting your password. 

If you are using a windows device then dowload [git](https://gitforwindows.org) and navigate to [stackoverflow](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994) to learn about using bash on windows.

After this, open VScode again and create a new terminal window. In the terminal type
`$ ssh cs15lsp23AA@ieng6.ucsd.edu`
where AA is replaced by the to letters accociated with your course account, this is found after logging into your account above before resetting your password. Then the terminal will prompt you for your newly reset password.
If its your first time connection to the server you will most likely be prompted with the following text, just type `yes`

```
⤇ ssh cs15lsp23@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
```

Next you'll see something that looks like this appear in the terminal
![Image](https://github.com/WillDiego/cse15l-lab-reports/blob/main/scr2.png)
At this point you should be connected to the remote server. If this does not work review the steps, if it still does not work you could contact one of course TAs.

## Step 3: Running Some Commands
Now that you're remotely connected you can try typing in commands. Some examples of commands to use are:
```
 cd ~
 cd
 ls -lat
 ls -a
 ```
 An example would be using `ls -lat` which would look something like this
 ![image](https://github.com/WillDiego/cse15l-lab-reports/blob/main/scr1.png)
 With this information you should be ready to remote connect and use commands in the remotely connected enviroment.
