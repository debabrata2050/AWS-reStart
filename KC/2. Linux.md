# Linux

## KC - An Introduction to Linux

#### 1. Which statement about the Linux operating system is true?
- [x] Linux is open source. ✅
- [ ] Linux is owned by an individual.
- [ ] Linux is based on the Microsoft Windows operating system.
- [ ] Linux is used only for desktop computers.

#### 2. Which component of the Linux operating system allocates the memory that is used to run applications?
- [ ] User interface
- [ ] Configuration files
- [x] Kernel ✅
- [ ] Shell

#### 3. What is a Linux daemon?
- [x] A program that provides a service and runs in the background ✅
- [ ] A hardware component that provides security services on a computer
- [ ] A program that manages the file system on a computer
- [ ] A server that controls the devices that are connected to other computers

#### 4. Which command enables you to review the manual page for the *hostname* command?
- [ ] ls hostname
- [ ] print hostname
- [ ] more hostname
- [x] man hostname ✅

#### 5. What are the main components of a Linux distribution? (Select TWO.)

- [x] Kernel ✅
- [ ] Paid support subscription
- [ ] Online tutorial videos
- [ ] Amazon Web Services (AWS) account registration
- [x] Complementary tools and applications ✅

***

## KC - Linux Command Line

#### 1. What is the name of the default Linux shell?
- [ ] Bat
- [ ] Korn
- [ ] C shell
- [x] Bash ✅

#### 2. Which keyboard key automatically completes commands in the default Linux shell?
- [ ] CTRL
- [ ] SHIFT
- [ ] ENTER
- [x] TAB ✅

#### 3. Which keyboard key retrieves the last command that you entered in the default Linux shell?
- [ ] INSERT
- [x] UP arrow ✅
- [ ] ESC
- [ ] BACKSPACE

#### 4. Which command displays the name of the account that you are logged in as in the default Linux shell?
- [ ] history
- [x] whoami ✅
- [ ] login
- [ ] wc

#### 5. Which command displays the name of the computer that you are logged in to in the default Linux shell?
- [ ] cal
- [ ] host
- [x] hostname ✅
- [ ] id

***

## KC - Users and Groups

#### 1. Which statements apply to setting user passwords? (Select TWO).
- [ ] Password characters must all be lowercase.
- [x] Users can reset their own passwords. ✅
- [ ] Passwords must be entered three times.
- [ ] Passwords must be eight characters in length.
- [x] Passwords are set with the passwd command. ✅

#### 2. Which permissions does a standard user have? (Select TWO).
- [ ] Control any service
- [ ] Manage any account
- [x] Access any files that the user has permissions for ✅
- [x] Control any files that the user owns ✅
- [ ] Manage the Linux kernel

#### 3. Which command gives you full administrative privileges and allows you to switch to the root user's environment?
- [ ] useradd
- [ ] sudo
- [ ] bash
- [x] su ✅
 
#### 4. Which command allows you to add a user to a group?
- [ ] groupadd
- [ ] sudo
- [ ] groupmod
- [x] usermod ✅
 
#### 5. Which statement is a best practice for using the root account?
- [ ] Always use the root account, and switch to a standard account only when you test the system.
- [ ] Allow only help desk users to use the root account.
- [x] Always log in as a standard user, and switch the user to the root account only when you must elevate permissions. ✅
- [ ] Share the root account password with all users, and monitor account usage by using logs.

***

## KC - Editing Files

#### 1. What is the default text editor for virtually all Linux distributions?
- [ ] Visio
- [x] Vim ✅
- [ ] gedit
- [ ] Notepad

#### 2. A systems administrator is editing a text file in Vim and is in the Insert mode. The administrator wants to exit the Insert mode and return to the Command mode. What keyboard key should the administrator press?
- [ ] TAB
- [x] ESC ✅
- [ ] ENTER
- [ ] SHIFT

#### 3. A developer is editing a file in Vim, and they want to save the file and exit the editor. Which command should the developer use?
- [x] :wq ✅
- [ ] i
- [ ] x
- [ ] /g

#### 4. A systems operator is editing a file in Vim, and they want to exit the editor without saving the file. Which command should the operator use?
- [ ] ESC
- [ ] :x
- [ ] :w
- [x] :q! ✅

#### 5. Which Linux text editor has a graphical user interface (GUI)?
- [ ] nano
- [x] gedit ✅
- [ ] vi
- [ ] Vim

***

## KC - Working with the File System

#### 1. Which statements about Linux file names are true? (Select TWO.)
- [ ] File names can contain spaces.
- [x] Extensions are optional. ✅
- [ ] Extensions are automatically mapped to applications.
- [x] File names are case sensitive. ✅
- [ ] Multiple files with the same name can exist in a directory.

#### 2. Which directory contains a user's personal files by default?
- [ ] /etc
- [x] /home ✅
- [ ] /var
- [ ] /dev

#### 3. Which command displays the absolute path to the user's current location in the file system?
- [ ] ср
- [ ] tail
- [x] pwd ✅
- [ ] cat

#### 4. Which command changes the current working directory to a different directory?
- [ ] mkdir
- [ ] mv
- [x] cd ✅
- [ ] rm

#### 5. A systems administrator must see a list of all files in the /var/log directory in long format. Which command and option should the administrator use?
- [ ] cat -names /var/log
- [ ] /var/log -la -ls
- [x] ls -la /var/log ✅
- [ ] cd /var/log

***

## KC - Working with Files

#### 1. Which option can you use with the find command to run a command on searched files?
- [ ] -delete
- [ ] -fprint
- [x] -exec ✅
- [ ] -user

#### 2. A Linux administrator downloaded a file from the internet. The administrator believes that the file is corrupted. Which Linux command can the administrator use to check whether a file is corrupted?
- [x] cksum ✅
- [ ] grep
- [ ] find
- [ ] diff

#### 3. A Linux administrator must compare and display the outputs of two different files. Which Linux command can the administrator use to compare the file outputs?
- [ ] df
- [ ] hash
- [ ] find
- [x] diff ✅

#### 4. Which statement about symbolic links is true?
- [x] Symbolic links point to a hard link, instead of the actual file. ✅
- [ ] Symbolic links can't link to any directory.
- [ ] If a symbolic link links to a file and the file is deleted, the link will still work.
- [ ] Symbolic links point to a file's inode.

#### 5. Which option for the tar command enables a user to create a tarball?
- [ ] -v tarball
- [ ] -xf tarball.tar
- [x] -cvf tarball.tar ✅
- [ ] -c tarball.tar

***

## KC - Managing File Permissions

#### 1. Which command allows the user to set permissions for files and directories?
- [x] chmod ✅
- [ ] chgrp
- [ ] su
- [ ] mask

#### 2. Which of the following is an example of Absolute mode?
- [x] chmod 757 filename ✅
- [ ] chmod
- [ ] chmod filename
- [ ] chmod a=r filename

#### 3. Which command displays the permissions for files and directories?
- [ ] ls
- [ ] ls -r
- [ ] ls -a
- [x] ls -l ✅

#### 4. Which command is used to change the user or group of a file or directory?
- [ ] umask
- [ ] chmod
- [ ] su
- [x] chown ✅

#### 5. Which statement reflects the principle of least privilege?
- [ ] Give access to all groups, and each group can decide which individual has access to each file.
- [x] Give the least number of users the least amount of file access first, and grant more permissions only when the user has a need. ✅
- [ ] Give a small number of users the most amount of access to all files.
- [ ] Give no access to any files for a large number of users, and give only the network engineer access to all files.

***

## KC - Working with Commands

#### 1. Wildcards are used to specify one to many unknown characters, or a set of limited and specific values in a search. What types of wild card characters does Bash recognize? (Select TWO.)
- [ ] #
- [ ] %
- [ ] &
- [x] * ✅
- [x] ? ✅

#### 2. Which of the following runs a series of three commands with a single command line?
- [ ] cd .. > rm *.csv > ls *.csv
- [x] cd .. ; rm *.csv ; ls *.csv ✅
- [ ] cd .. --add rm *.csv --add ls *.csv
- [ ] cd .. | rm *.csv | ls *.csv

#### 3. A developer is troubleshooting an issue and wants to check the log file /var/log/ secure.log for any failures. Which command syntax is available to find if the log file contains the word "fail"?
- [x] grep fail /var/log/secure.log ✅
- [ ] find fail /var/log/secure.log
- [ ] grep fail | find /var/log/secure.log
- [ ] find fail -name /var/log/secure.log

#### 4. What is the *sed* command?
- [ ] A tool to manage directories
- [ ] An editor similar to vi
- [ ] A search tool
- [x] A non interactive text editor ✅

#### 5. Which of the following are output redirectors that enable redirecting the standard output? (Select TWO.)
- [ ] |
- [x] >> ✅
- [x] > ✅
- [ ] <
- [ ] <<

***

## KC - Managing Processes

#### 1. A software developer is having issues with a process that runs on a Linux host. The application is not responding. The developer decides to end the process by using the kill command, which requires the process ID (PID). Which command can the developer use to retrieve the PID?
- [ ] echo <process_name>
- [ ] ps <process_name>
- [ ] jobs <process_name>
- [x] ps -ef ✅

#### 2. Which commands list the process IDs (PIDs) for the running processes on a Linux host? (Select TWO.)
- [ ] Crontab
- [ ] ls
- [ ] echo
- [x] ps ✅
- [x] pidof ✅

#### 3. A systems administrator wants to schedule some tasks so that they run automatically. Which commands enable the administrator to schedule automatic tasks? (Select TWO.)
- [ ] jobs
- [ ] ps
- [x] at ✅
- [ ] time
- [x] crontab ✅

#### 4. Which kill command signal will immediately stop a process with NO graceful exit?
- [ ] -19 SIGSTOP
- [x] -9 SIGKILL ✅
- [ ] -31 SIGSYS
- [ ] -15 SIGTERM

#### 5. Which state indicates that a process is waiting to be assigned?
- [ ] Start
- [x] Ready ✅
- [ ] Running
- [ ] Waiting

***

## KC - Managing Services

#### 1. Which service can AWS customers use to monitor AWS services and resources?
- [ ] AWS Control Tower
- [ ] Amazon Simple Notification Service (Amazon SNS)
- [x] Amazon CloudWatch ✅
- [ ] Amazon Elastic Compute Cloud (Amazon EC2)

#### 2. Which command lists all active services?
- [x] systemctl list-units --type=service --state=active ✅
- [ ] systemctl list-units --type=service
- [ ] systemctl status
- [ ] systemctl

#### 3. Which command displays the usage of virtual memory?
- [ ] lshw
- [x] vmstat ✅
- [ ] free
- [ ] fdisk

#### 4. Which command displays the amount of free disk space?
- [x] df ✅
- [ ] ls
- [ ] cat
- [ ] mkfs

#### 5. Which system-performance command monitors how much physical memory is available?
- [ ] lscpu
- [ ] cat /proc/partitions
- [ ] ps
- [x] free ✅

***

## KC - The Bash Shell

#### 1. What is a variable?
- [x] A variable is a value that's substituted into the script or command. ✅
- [ ] A variable is strictly a value that contains a letter.
- [ ] A variable is strictly a value that contains a number.
- [ ] A variable is a value that contains a ampersand (&).

#### 2. Consider the following command: echo $HOME. Which portion of the command is the variable?
- [ ] $
- [x] HOME ✅
- [ ] echo
- [ ] The command has no variable

#### 3. A developer is testing a Bash script and wants to display information as the script runs. Which command should the developer use?
- [x] echo ✅
- [ ] chksum
- [ ] run
- [ ] env


#### 4. A user would like to change how their aliases are configured. Which file should the user change to alter their configurations?
- [ ] .passwd file
- [ ] .profile file
- [x] .bashrc file ✅
- [ ] host.conf file

#### 5. Which environment variable is used to indicate the location of the commands?
- [x] $PATH ✅
- [ ] $HOME
- [ ] $USER
- [ ] $SHELL

***

## KC - Bash Shell Scripts

#### 1. Why might an administrator create a Bash shell script? (Select TWO.)
- [x] To automate a repetitive task. ✅
- [ ] To use the built-in data validation feature of the Bash shell when they run a task.
- [ ] To document commonly used commands in a single file.
- [ ] To run a task that requires elevated permissions.
- [x] To ensure that a task runs correctly and consistently. ✅


#### 2. Which of the following displays the correct syntax for the first line of a bash script to make it executable?
- [x] #!/bin/bash ✅
- [ ] #!/bash
- [ ] #!/bin
- [ ] #!

#### 3. Consider the following statement: sum=$(($2 + $4)). Which parts of the statement represent the arguments?
- [ ] $() and ($2 + $4) are the arguments.
- [ ] $ and () are the arguments.
- [x] $2 and $4 are the arguments. ✅
- [ ] sum and ($2 + $4) are the arguments.

#### 4. Which command causes a Bash script to stop running and exit the shell?
- [x] exit ✅
- [ ] kill
- [ ] return
- [ ] wait

#### 5. Which conditional statement defines two courses of action?
- [ ] for
- [x] if - else ✅
- [ ] while
- [ ] if

***

## KC - Software Management

#### 1. Which components are part of a package? (Select THREE.)
- [x] Installation instructions ✅
- [ ] User emails
- [x] Pre-compiled code ✅
- [ ] Kernel
- [ ] Feedback text
- [x] Documentation ✅

#### 2. Which command updates a Red Hat Package Manager (RPM) package?
- [ ] apt-get update
- [x] yum update <package name> ✅
- [ ] yum search <package name>
- [ ] yum check-update <package name>

#### 3. Which command enables a user to display specific packages?
- [ ] yum list available
- [ ] yum list installed
- [x] yum list installed | grep ✅
- [ ] yum list installed httpd

#### 4. Which locations can be used for storing repositories? (Select THREE.)
- [ ] Flash drive
- [x] Local hard disk drive ✅
- [ ] Random access memory (RAM)
- [ ] Temporary storage on the cloud
- [x] Internal server ✅
- [x] Online vendor site ✅

#### 5. Which program is a common utility for downloading files from a server?
- [ ] vim
- [ ] gzip
- [x] wget ✅
- [ ] find

***

## KC - Managing Log Files

#### 1. In Linux distributions, where are log files normally stored?
- [ ] /boot
- [ ] /dns
- [ ] /bin
- [x] /var/log ✅

#### 2. Which Syslog level shows the highest level of severity for an event?
- [ ] Alert (alert)
- [ ] Debug(debug)
- [x] Emergency (emerg) ✅
- [ ] Warning (warn)

#### 3. Which statements about a log file are correct? (Select TWO.)
- [ ] A log file is automatically rotated by default.
- [ ] A log file can only be viewed using an editor.
- [x] A log file can help troubleshoot issues. ✅
- [ ] A service-level agreement (SLA) is a is a type of log file.
- [x] The size and number of log files on a server can quickly increase. ✅

#### 4. Which two commands display the first 10 lines and last 10 lines of a file? (Select TWO.)
- [ ] history
- [x] tail ✅
- [ ] first
- [x] head ✅
- [ ] last

#### 5. A Linux systems administrator must perform security audits, which is a routine administration task. During a security audit, the administrator must determine which recent users have logged in to the system. Which command enables the administrator to show the users who logged in recently?
- [ ] nslookup
- [x] lastlog ✅
- [ ] users
- [ ] locate
