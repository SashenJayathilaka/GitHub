# GitHub
### Git commands


## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/SashenJayathilaka/Coding_Website/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

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

### Git Tags
##### Checkout the branch where you want to create the tag
git checkout "branch name"
```
git checkout master
```
##### Create tag with some name
git tag "tag name"
```
 git tag v1.0
```
git tag -a v1.0 -m "ver 1 of .."  (to create annotated tags) 
##### Display tags
```
git tag
```
##### Push tags to remote
```
git push origin v1.0
```
```
git push origin --tags
```
```
git push --tags 
```
(to push all tags at once)
##### Delete tags 
###### delete tags from local
```
git tag -d v1.0
```
```
git tag --delete v1.0
```
###### delete tags from remote
```
git push origin -d v1.0
```
```
git push origin --delete v1.0
```
```
git push origin :v1.0
```
###### delete multiple tags at once
local
```
git tag -d v1.0 v1.1
```
remote
```
git push origin -d v1.0 v1.1
```
##### Checking out TAGS
We cannot checkout tags in git <br>
We can create a branch from a tag and checkout the branch <br>
git checkout -b "branch name" "tag name"
```
git checkout -b ReleaseVer1 v1.0
```
###### Creating TAGS from past commits
git tag "tag name" "reference of commit"
```
git tag  v1.2 5fcdb03
```
