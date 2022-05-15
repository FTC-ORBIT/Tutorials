### This is a brief explanation of all of the basic git commands:

- git config
Sets configuration values for your user name, email, gpg key, preferred diff algorithm, file formats and more. Examples:

`git config --global user.name "My Name"`
`git config --global user.email "user@domain.com"`

- git init
Initializes a git repository – creates the initial .git directory in a new or in an existing project. Example:

`git init`

`Initialized empty Git repository in /home/customer/GIT/.git/ `

- git clone
Creates a GIT repository copy from a remote source. Also adds the original location as a remote so you can fetch from it again and push to it if you have permissions. Example:

`git clone git@github.com:user/test.git `

- git add
Adds files changes in your working directory to your index. Example:

`git add . `

- git rm
Removes files from your index and your working directory so they will not be tracked. Example:

`git rm filename`

- git commit
Takes all of the changes written in the index, creates a new commit object pointing to it and sets the branch to point to that new commit. Examples:

`git commit -m ‘committing added changes’`

`git commit -a -m ‘committing all changes, equals to git add and git commit’`

-git status
Shows you the status of files in the index versus the working directory. It will list out files that are untracked (only in your working directory), modified (tracked but not yet updated in your index), and staged (added to your index and ready for committing). Example:

`git status`
 
 `On branch master 
 Initial commit 
 Untracked files: 
 (use "git add <file>..." to include in what will be committed) #
 `

- git branch
Lists existing branches, including remote branches, if ‘-a’ is provided. Creates a new branch if a branch name is provided. Example:

`git branch -a * master remotes/origin/master`

- git merge
Merges one or more branches into your current branch and automatically creates a new commit if there are no conflicts. Example:

`git merge newbranchversion`

- git reset
Resets your index and working directory to the state of your last commit. Example:

`git reset --hard HEAD`

- git tag
Tags a specific commit with a simple, human-readable handle that never moves. Example:

`git tag -a v1.0 -m 'this is version 1.0 tag'`

- git pull
Fetches the files from the remote repository and merges it with your local one. Example:

`git pull origin`

- git push
Pushes all the modified local objects to the remote repository and advances its branches. Example:

`git push origin master`

- git remote
Shows all the remote versions of your repository. Example:

`git remote origin`

- git log
Shows a listing of commits on a branch including the corresponding details. Example:

`git log commit`

`84f241e8a0d768fb37ff7ad40e294b61a99a0abe Author: User <user@domain.com> Date: Mon May 3 09:24:05 2010 +0300 first commit`

- git diff
Generates patch files or statistics of differences between paths or files in your git repository, or your index or your working directory. Example:

`git diff`

### For practice visit this website: https://learngitbranching.js.org/
