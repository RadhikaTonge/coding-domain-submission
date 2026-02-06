# Task 1 Learning basic Linux Commands

What is exactly Linux?
Linux is an operating system just like Windows or macOS.An operating system is the main software that talks to your hardware such as CPU,RAM,keyboard,screen, etc.It lets
you to run programs in your device.Linux is a free and open source operating system thta is anyone can see and modify its code.It is very stable and it rarely crashes.
Linux is very powerful, it is used in servers,clouds,robotics,AI,hacking,Android,etc.Most of the servers on the internet run on Linux. Android is build on Linux kernel.
Robotics boards such as Raspberry Pi,Jetson,servers for ROS use Linux.Linux expects you to talk it using commands.

Linux does not use C:\,D:\ like windows.Everything starts from root /.

Common folders that are used in Linux are as follows
     Folder                                      Meaning
 1.  /                                           Root(top of everything)
 2.  /home                                       User files(like Documents)
 3.  /home/username                              Your personal space
 4.  /bin                                        Basic commands
 5.  /etc                                        Configuration files
 6.  /usr                                        Installed software
 7.  /var                                        Logs and changing files


Basic Linux Commands

1. pwd
   This shows your current location.This command gives answer to the question "Where am I?"
   Example output:
   /home/john

2. ls
   This command give us lists of files and folders present in the current directory.It gives answer to the question "What's here?"
   Example output:
   ls
   linux_commands.md

3. ls -l
   This command gives us detailed listing or long list of files and folders present in the directory.

4. ls -a
   This command shows hidden files.Hidden files start with dot.

5. ls -la
   This command gives hidden as well as detailed files and folders in the directory.

6. cd
   This command is used in changing of directory.This command helps to move between folders.
   Example output:
   cd Task-1-Linux

7. cd..
   this command is used to go back to your parent folder of your current directory.
   Example output:
   If you are in the folder
   Desktop/College/Robotics
   using command
   cd..
   Desktop/College

8. cd ~
   This command is called Tilde,which is used to go back to your home directory.

9. cd /
   This command is used to go to root.

10. mkdir
   This command is used to create a folder.
   Example output:
   mkdir test
   Creates a folder named test.

11. rmdir
   This command is used to delete the empty folder.It is necessary that the folder should be empty.

12. touch
   Creates an empty file.
   Example output:
   touch file.txt

13. cat
   This command displays content of the file.It reads the file.

14. rm
   This command is used to delete the files present in directory.

15. cp
   This command is used to copy files from one folder to other.

16. mv
   This command is used to move or rename the file.

17. clear
   This command is used to clear the screen.It does not delete anything.

Conclusion
In this task, I learned and practiced basic Linux commands using Git Bash without installing Linux.Through this task, I learned basic Linux commands used for file and directory management. These commands are essential for development and version control.


