# GitHub Tutorial

_by Si Ting Chen_

---
## Git vs. GitHub
**_Git_**
* Revision control keep ”snapshots” of code (Timeline: remember what you change)

**_GitHub_**
* Store code in the cloud(server that connect to the internet)
* Visually track change
* Easily collaborate on files

**_What is the difference between Git and Github?_**  
* Git is use for revision control system, which manage to keep ”snapshots” of code and Github is a cloud-based hosting service that lets you manage Git repositories.

---
## Initial Setup
[How to make a GitHub Account](https://github.com/)
* Click on the GitHub website on the top.
* Click Sign-Up
* Filled in the information (Username, Email, Password)
  * Password must be at least 8 character including a number and a lowercase letter.

[How to set up your IDE](https://ide.cs50.io/)
* Log into your github account 
* Click on the IDE website on the top. 
* Click Sigh in with GitHub from the blue box on the left.  
 **or**
* Since the IDE is connected to your github account.
* Type (ide.cs50/your username for github/ide) to login.  

---
## Repository Setup

###### When setting up repository change: 

1. Make a folder in your parent folder by using "mdkir".
2. When you are in the directory type **git init** to open a new repository so you can make change inside the repository.
3. Type c9 to open file 
4. Type **git add .** to add all the revelant in the files.
5. Type **git commit -m "your message"** to save change in folder.
6. Type **_git push_** to commit all the meassge you make in github.

###### To connect remote repository in github:
 
1. Go to github and sign in.
2. Click on the "new repository" on the top right corner from the "+" icon.
3. click "create repository"
4. Make a name in your repository.
5. Make sure you are in the "SSH key" link.
6. Go to your ide50 cd in to the repository that you just make.
7. Type "git remote add origin git@github.com:<Your github account name>/<Your repository name>.git
8. type git push -u origin master ths way whatever you write on the ide50 will connect to your repository on your github page.

---
## Workflow & Commands

**_init_**    
* initializes git in the directory which now is call a **repository** for vision control.
* only do this once at the beginning (main folder).

**_status_**    
* The git status command displays the state of the working directory and the staging area.
* Git status helps keep track of what change have you staged.

**_add_**      
* It is use to adds a change in the working directory to the staging area.
* Git add is to help indicate or modifies the project you did works.

**_commit_**  
* Git commit is used to save changes in your local repository.

**_push_**    
* To push committed changes to github
* Upload repository to github.

###### Ongoing Workflow:

1. **"cd"** into the folder that you want to work on.
2. **"c9 <file name>"** into the file that you want to work on.
3. make edit in the file.
4. **"git add."** so it ready to commit
5. **"git status"** to make sure the change is modified.(green color)
6. **"git commit"** -m "your message" 
7. **"git push"** to transfer all commit to your github.
8. repeat from **step 4** a certain amount of time when you want to save change.



---
## Rolling Back Changes