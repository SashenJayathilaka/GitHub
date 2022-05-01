# GitHub
### Git commands


#### Push Repositories
##### Initialize repository in project folder
```
git init 
```
##### Add files to local repository
```
git add . or git add <file names> 
```
##### (Add comments in Nano or vim) - Commit repository
```
git commit -m "< message >" or git commit 
```
##### Show all files which have changes to commit
```
git status
```
##### Add local repository to remote repository
```
git remote add origin < remote repository URL > 
```
##### Push local changes to remote
```
git push origin master 
```
##### If push was successful?
```
git push -f origin master
```
### How to create a new branch in git 
##### Example for creating a new branch named myNewBranch
```
git checkout -b myNewBranch
```
##### First Push
```
git push --set-upstream origin myNewBranch
```
### Deleting a branch LOCALLY
##### Deleting a branch locally
```
git branch -d localBranchName
```
##### Delete branch remotely
```
git push origin --delete remoteBranchName
```
##### Refresh branch list
```
git fetch -p
```
##### Force delete if getting merge error
```
git branch -D local_branch_name
```

##### Removing the last commit
```
git reset --hard HEAD^
git push origin -f
```
