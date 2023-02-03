# git-first-task

THIS SHOULD ONLY APPEAR IN UAT

# This is my first repository, it contains basic git commands.
# First clone remote repository onto local machine (only need to do 1x)
git clone GitHubURL


# Then make changes to local repository, i.e. add new files, edit Readme.md etc.

# Then make changes to local repository, i.e. add new files, edit Readme.md etc.

# show status of the current repository inc the files that have been modified
# and need to be commited. 
# First time you do this with new changes, will be in RED
git status

# Need to be in the local repository where you are editing the Readme.md file
# Add all the change in your directory to git in your local repository 
# where it's creating a local stage version of what is on your remote repository.
git add . 

# Second time you do this with new changes, should be in GREEN (denoting they've
# been added already). Will show that changes have been added to local git repository 
# and is now yet to be commited on local repository.
git status


# commit your change to the local repository. 
# Save a snapshot of the changes in the staging area with a descriptive message 
# "[message goes here]"
# First time users will need to verify who you are. git config --global user.email "your email"
git commit -m ""

# Displays commit history on local repository.
git log

# Then you will push your changes to remote branch so others can see your 
# changes. Pushing your changes into remote branch and remote origin.
git push origin branchName


# Wk 1, Lec 3 - 01/18/23

# Displays list of branches on your local repository system.
git branch

# Create a new branch with given name, -b will create new branch. 
# (flag to indicate branch name)
git checkout -b branchName

# Switch to a different branch
git checkout branchName


# Merge new changes from sourceBranch to targetBranch. Need to 
# navigate FIRST to target branch (branch you are seeking to 
# update with new changes). Ex: develop --> uat --> main
# -> git checkout targetBranch
git merge sourceBranch

# then you need push those new changes on the targetBranch into 
# the remote repository.
git push origin targetBranch

# git pull is an alternative to merge (except you must first push 
# new code remotely to do this). Unlike MERGE, PULL cannot pull locally, 
# has to be pulling from remote.
git pull sourceBranch(remote)