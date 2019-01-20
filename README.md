# 1.1-git-exercise
UVic Robotics Integration 1.1 exercise
This is a simple markdown manual to know how to write it: https://guides.github.com/features/mastering-markdown/

## Git concepts
* Repository: Project space where files and history of the development are stored
* Working copy: Repository files at your local machine
* Branch: a development path, linked to the repository
* Commit: Picture of the repository files at a given moment
* Checkout: Change your working copy to a given commit or branch
* Push/Pull: Upload/Download to/from repository
* Merge: Incorporate a set of commits of branch A to branch B
* Issue: A problem, bug, new feature, we want/have to work with
* Merge/Pull Request: Request of merging a branch/commit to another branch
* Fork: Unlinked development path, which creates an independent repository

## Important commands: (All this data is from git page: https://git-scm.com/docs)
* Clone a repository: **git clone {url pointing to repository (.git)}**
* Add file after create it: **git add {file}**
* Remove file from local repository: **git rm {file}**
* Move/Rename file from local repository: **git mv {file}**
* Check the status of your repository: **git status**
* Check the repository branch log: **git log**
* Commit the local changes: **git commit -am "{message for this commit}"**
* Push the local repository to the remote repository (master branch): **git push origin master**
* List branches: **git branch**
* Create a new branch: **git branch {branch name}**
* Switch to other branch: **git checkout {branch name}**
* Merge branches:
    1. Go to the destination branch: **git checkout {branch name}**
    1. Merge the branch: **git merge {branch name you want to merge}**
* Delete a branch: **git branch --delete {branch name}**
* Delete a remote branch: **git push origin --delete {branch name}**

## Remember your password instead type every time
To get your Git client to remember your username and password, and avoid re-entering it every time you access your repository over HTTPS, you can issue the following command to your Git client:
```
git config --global credential.helper cache
```
If you wanted Git to remember it for longer, you can do so by specifying a --timeout=:
```
git config --global credential.helper "cache --timeout=3600"
