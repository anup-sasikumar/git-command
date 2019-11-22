#This is a practice repository having all GIT commands

##Commands Used:
- git init : creates a new GIT repository
- git status : compares working directory, staging area and current branch
- git add : add all the changes at that point in time from working directory to staging area
- git commit : commit the changes from staging area to the current branch
- git config : set or get the configuration parameters
- git log : show history or log of project commits
- git branch -c name : creates a new branch with given name
- git branch : lists all the branches in the repository with an indicator on current branch
- git checkout name : check out or switches to the branch name
- git checkout -b : creates a new branch and switches to it

##To understand stash
- git stash : stores the uncommitted changes from working directory and index state as WIP
- git stash list : lists the uncommitted changes in the current branch
- git stash pop : apply the uncommitted changes back to the working directory


##Merge operation brings changes from one branch into another
- git merge : Merge changes from different branches

A fast-forward merge happens when the target branch (merged_branch) was branched from the current branch (master) and there are no changes to current branch since then.
An automatic merge happens when the two histories have diverged, but GIT is able to reconcile them into one set of changes. This creates a new commit on current branch (master)
