# GitHub Tutorial

_by Si Ting Chen_

---
## Git vs. GitHub
**_Git_**
* Revision control keep ”snapshots” of code (Timeline: remember what you change)

**_GitHub_**
* Store code in the cloud (server that connect to the internet)
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
4. Type **_git add ._** to add all the revelant in the files.
5. Type **_git commit -m "your message"_** to save change in folder.
6. Type **_git push_** to commit all the meassge you make in github.

###### To connect remote repository in github:
 
1. Go to github and sign in.
2. Click on the "new repository" on the top right corner from the "+" icon.
3. Click "create repository"
4. Make a name in your repository.
5. Make sure you are in the "SSH key" link.
6. Go to your ide50 cd in to the repository that you just make.
7. Type "git remote add origin git@github.com/username/new_repo
8. Type git push -u origin master ths way whatever you write on the ide50 will connect to your repository on your github page.

---
## Workflow & Commands

**_init_**    
* Initializes git in the directory which now is call a **repository** for vision control.
* Only do this once at the beginning (main folder).

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

**_log_**
* Git log is use to see your past commit.

**_diff_**
* Git diff is use to see the difference between your current code and the previous commits.

**_pull_**
* Git pull is use to bring any change from the remote repo “down” to the local repo.

**_cd_**
* cd (folder name) - goes to that folder
* cd .. - goes to the parent directory
* cd ~ - goes to the root directory

**_touch_**
* touch <files name>.txt - creates a file

###### Ongoing Workflow:

1. Type **"cd"** into the folder that you want to work on.
2. Type **"c9 <file name>"** into the file that you want to work on.
3. Make edit in the file.
4. Type **"git add."** so it ready to commit
5. Type **"git status"** to make sure the change is modified.(green color)
6. Type **"git commit"** -m "your message" 
7. Type **"git push"** to transfer all commit to your github.
8. Repeat from **step 4** a certain amount of time when you want to save change.

---
## Rolling Back Changes

**_undo an "edit"_**  
When make change  
* git checkout -- (file name): to undo any edit in the last commit

**_undo a "git add"_**      
To get green modified to red modified when make another change 
* git reset HEAD (file name): to undo change from adding

**_undo a "git commit"_**  
To save change
* git reset --soft HEAD~1: to remove commit you do in the last commit

**_undo a "git push"_**  
To upload change 
* Type **"git log"** to see which commit you want to go back.
* Type **"git revert"** to get to the page that you have commit that time.
* Type **"git reset--hard"** is a destructive operation for uncommitted changes.
* Type **"git push orgin master"** to push the commit that you revert from local branch to remote.
