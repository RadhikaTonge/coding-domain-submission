What is Git?

Git is a version control system.


Lets imagine that we are working on a project:
We write some code today for the project.tomorrow we make some changes into the code.Day after tomorrow we remove some part of the code.Now we want the older version of code back.We want to see what changes we exactly did it the code.We also do not want to lose the previous version of code,and want it to store somewhere.

This it what exactly Git does.

Git keeps track of changes you made in your project files over time.It saves versions of your project.It lets you go back to older versions of your code or project.It helps multiple people work on the same project without conflict.Git works locally on our computer.

Application of Git

Git is used in software development projects,it is used in robotics projects,in different companies.

What is GitHub?
GitHub is a website that works online,github stores our projects whereas git tracks the record of our code or project.git hub is used in brower as it works online. 

Simply,
Git = tool that tracks your project
GitHub = online place where your Git projects are stored

 Basic Git Terminology

1. Repository (Repo)
A repository is a project folder tracked by Git.

2. Commit
A commit is like a save point.It stores changes with a message.

3. Branch
A branch is a separate line of development.(Default branch is usually main.)

4. Remote
Remote means the online GitHub repository.

Basic Git Commands 

1. git --version
This command checks if Git is installed in our device.

2. git init
this command initializes Git in a folder.Git start tracking this folder.After this, our folder becomes a Git repository.

3. git status
This command shows current state of files.Shows the current status of our file, that is where it is located.It tells us which files are new and which files are modified.It tells what is staged.


4. git add
This command adds files to staging area (preparing for commit).For adding one file git add file_name is used and for adding all the files git add . command is used.

5. git commit
This command is used to saves changes within a message.The message you wrote should explain what you did.
Example
git commit -m "Initial commit"
"Added Linux commands file"

6. git log
This command shows commit history.After writing this command you can see who commited it,when it was commited,what was the commiting message.

7. Common Git Push Commands
git init
git status
git add .
git commit -m "message"
git remote add origin <repo-url>
git push -u origin main

First, we create a project folder on our computer and place all required files inside it. This folder contains the work that we want to upload to GitHub.

Next, we open the terminal inside this folder and initialize Git. Initializing Git means we are telling Git to start tracking all the files and changes inside this folder. Once Git is initialized, the folder becomes a Git repository on our local system.

After that, Git checks the status of the folder to see which files are new or modified. All the required files are then added to the staging area. The staging area is like a preparation step where we select which files should be saved in the next version.

Once the files are staged, we create a commit. A commit is a saved snapshot of the folder at that moment, along with a message that describes what the work contains. This commit acts as a checkpoint and records the current state of the project.

Then, the local Git repository is connected to a remote repository on GitHub. This step links our computer’s folder with the online repository so that Git knows where to upload the project.

Finally, the committed files are pushed to GitHub. Pushing means sending the saved version of the folder from the local system to the remote repository. After this step, the entire folder and its contents become visible on GitHub, confirming that the upload was successful.

By using the above process we can push our folder to Github into our repository.