## Download from Download - https://git-scm.com/download/
- Access GitHub using - https://github.com/

## Setup user profile for communication with GitHub:
-	git config --global user.name "<name>"
-	git config --global user.email "<email-id>"

## Basic GIT commands:
- git init : initialises a new GIT repository. This will initialize a .git file in the folder
- git status : compares working directory, staging area and current branch
- git add : add all the changes at that point in time from local or working directory to staging area
- git commit : commit the changes from staging area to the current branch
- git config : set or get the configuration parameters
- git log : show history or log of project commits
- git log <branch> : shows the history of all commits for the passed branch
- git log <commit-ref> : shows the history of all commits prior to passed commit reference
- git log --all : shows the history of all commits for the entire repository
- $ git log --author “<name>” : shows the history of all commits by author on the current branch
- $ git log --since “<date>” : shows the history of all commits by period on the current branch
- $ git log --until “<date>” : shows the history of all commits till date on the current branch
- git show <commit-ref> : shows the history and differences introduced by commit reference
- git diff : shows the difference between working directory and HEAD
- git diff <ref> : shows the difference working directory and commit reference
- git diff --cached : shows the difference working directory and staging area ready to be committed

## GIT Remote Repository (origin)
# To set remote to add remote (origin) (for new project)
- git remote add origin <git-url> : To set remote by adding the remote <origin> to specified repository <git-url>
- git remote -v : list remote repositories
- git push -u <remote> <branch> : push <branch> to <remote> and set default upstream for <branch>
- git fetch : fetches files from remote origin master to tracking branch
- git merge : merges the changes in tracking branch to local branch
- git pull origin master : pull the code from origin for master
- git clone <git-url>  : Clone the project if already available

## Branching - GIT follows a tree structure - Root will be the master branches and we create sub-branches as a copy of master branch
- git branch -c <branch-name> : creates a new branch <branch-name>
- git checkout <branch-name> : check out or switch to the <branch-name>
- git checkout -b <branch-name> : create a new branch <branch-name> and switch to it
- git branch : lists all the branches in the repository with an indicator on current branch
- git push -u origin <branch-name>
- git pull origin <branch-name>
- git branch -d <branch-name> : deletes the branch

## Merge Operation - brings changes from source branch(DEV) to destination branch(master)
- git checkout <destination-branch>
- git pull origin <destination-branch> 
- git merge <source-branch> : merge changes from source branch to destination branch

## Merge Conflict - Stash and Unstash
# A commit accepts files only from stash and GitHub only accepts code which is in commit state
- git stash : stores the uncommitted changes from working directory and index state as WIP
- git stash list : lists the uncommitted changes in the current branch
- git stash pop : apply the uncommitted changes back to the working directory

A fast-forward merge happens when the target branch (merged_branch) was branched from the current branch (master) and there are no changes to current branch since then.
An automatic merge happens when the two histories have diverged, but GIT is able to reconcile them into one set of changes. This creates a new commit on current branch (master)
