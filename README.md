Git Workflow
==
##0. Set up Git (Mac OS)
To use Sublime as a default editor:
>`git config --global core.editor "sublime -n -w"`

##1. Initialize git repository
###a. Create a local repository from existing directory
Go to directory where you want to create git repository: 
>`git init`  

###b. Clone a remote repository to local machine
If you have a remote repository you want to clone to your local machine:
>`git clone http://<url for your remote repository>.git`

---
If you want to clone the repository into a directory named other than the name of the repository:
>`git clone http://<url for your remote repository>.git <name of directory>`

To check status of your git repository:
>`git status`  

##2. Track files
###a. Save changes
To start tracking file:
>`git add <file name>`  

---
To see what you’ve changed but not yet staged:
>`git diff`

---
To commit changes:
>`git commit`

---
To remove file:
>`git rm <file name>`

---
To view the commit history:
>`git log`

-p shows the diff in the commit, -2 outputs only the last 2 commits:
>`git log -p -2`

###b. Undo changes
If you want to try that commit again:
>`git commit --amend`

To unstage a staged files:
>`git reset HEAD <file name>`

To revert file to the last commit:
>`git checkout -- <file name>`

##3. Work with a remote repository
To fetch from a remote repository:
>`git fetch <remote name (origin)>`

To push to a remote repository:
>`git push <remote name (origin)> <branch name (master)>`

##4. Work with branches
###a. Create branches and modify files
To create / switch to a branch:
>`git branch <branch name>`

Shortcut for creating new branch and switching to it:
>`git checkout -b <branch name>`

---
To merge changes made in the specified branch into the branch that you are currently in:
>`git merge <branch name>`

---
To delete a branch:
>`git branch -d <branch name>`

###b. Resolve merge conflict
