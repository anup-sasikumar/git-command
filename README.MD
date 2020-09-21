# Download from Download - https://git-scm.com/download/
# Access GitHub using - https://github.com/

# Setup user profile for communication with GitHub:
-	git config --global user.name "<name>"
-	git config --global user.email "<email-id>"

#This is a practice repository having all GIT commands

##Commands Used:
- git init : initialises a new GIT repository. This will initialize a .git file in the folder
- git status : compares working directory, staging area and current branch
# A commit accepts files only from staging area and GitHub only accepts code which is in commit state
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
- git branch -c name : creates a new branch with given name
- git branch : lists all the branches in the repository with an indicator on current branch
- git checkout name : check out or switches to the branch name
- git checkout -b : creates a new branch and switches to it

#To understand stash
#A commit accepts files only from stash and GitHub only accepts code which is in commit state
- git stash : stores the uncommitted changes from working directory and index state as WIP
- git stash list : lists the uncommitted changes in the current branch
- git stash pop : apply the uncommitted changes back to the working directory


##Merge operation brings changes from one branch into another
- git merge : merge changes from different branches

##GIT Remote
# To set remote to add remote (origin) (for new project)
- git remote add origin <git-url> : To set remote by adding the remote <origin> to specified repository <git-url>
- git remote -v : list remote repositories
- git push -u <remote> <branch> : push <branch> to <remote> and set default upstream for <branch>
- git fetch : fetches files from remote origin master to tracking branch
- git merge : merges the changes in tracking branch to local branch
- git pull : fetch and merge
- git clone <git-url>  : Clone the project if already available

A fast-forward merge happens when the target branch (merged_branch) was branched from the current branch (master) and there are no changes to current branch since then.
An automatic merge happens when the two histories have diverged, but GIT is able to reconcile them into one set of changes. This creates a new commit on current branch (master)
