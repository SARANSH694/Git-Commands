# Git Commands

**A list of important and commonly used Git commands**

## Check Version : 
| Command | Description |
| ------- | ----------- |
| `git --version` | Check version of Git |
___

## Set & Check Configuration Values : 
| Command | Description |
| ------- | ----------- |
| `git config --global user.name "your username"` | Configure username |
| `git config --global user.email "your email"` | Configure email |
| `git config --list` | To ckeck Configuration Values |
___

## Need Help : 
| Command | Description |
| ------- | ----------- |
| `git help <verb> OR git <verb> --help` | To get help menu |
___

# For local repository :-

## For local repository tracking :
| Command | Description |
| ------- | ----------- |
| `git init` | To initialize git |
| `rm -rf .git` | To stop tracking |
| `git status` | Check status |
___

## For `.gitignore` file :
| Command | Description |
| ------- | ----------- |
| `touch .gitignore` | To make a gitignore file |

>`.gitignore` file contains name of the files which we donot want to be tracked or uploaded to the github.
___

>**Working directory is where untracked and modified files will be and it will list those when we run `git status` command.**

>**Staging area is where we can organize what we want to be commited to our repositories.**
___

## Add & Remove files to staging area :
| Command | Description |
| ------- | ----------- |
| `git add -A` | To add all files |
| `git add filename` | To add a specific file |
| `git reset` | To remove all files |
| `git reset filename` | To remove a specific file |
___

## To commit and view commit :
| Command | Description |
| ------- | ----------- |
| `git commit -m "Description"` | To commit to repository |
| `git log` | To view the commit |
___

# For Remote Repositories :-

## Cloning & Viewing information of remote repository :
| Command | Description |
| ------- | ----------- |
| `git clone https://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |
| `git remote -v` | It lists location of machine and repository |
| `git branch -a` | It will list all branches in our repository |
___

## Push and Pull changes :
| Command | Description |
| ------- | ----------- |
| `git pull origin branch_name` | It pulls all the changes made to the repository after the last time we pulled from the repository |
| `git push origin branch_name` | It pushes changes to the branch |

**Steps :-**
>Commit changes locally first
- `git diff` (Shows the changes made to the code)
- `git status`
- `git add -A`
- `git status`
- `git commit -m "Description"`
- `git pull origin master`
- `git push origin master`

## Create a branch :
| Command | Description |
| ------- | ----------- |
| `git branch branch_name` | To create new branch |
| `git checkout branch_name` | To switch to desired branch |
| `git branch -a` | To check all branches |
___

## Push and Pull branch to remote repository :
| Command | Description |
| ------- | ----------- |
| `git push -u origin branch_name` | To push branch to remote repository |
| `git checkout branch_name` | To switch to desired branch |
| `git branch` | To check all branches |
___

## Merge branches :
| Command | Description |
| ------- | ----------- |
| `git merge branch_name` | To merge branch with master branch |

**Steps :-**
- `git checkout master` 
- `git pull origin master`
- `git merge branch_name`
- `git push origin master`
___

## Delete branch :
| Command | Description |
| ------- | ----------- |
| `git -d branch_name` | To delete a branch |

**Steps :-**
- `git branch --merged` 
- `git branch -d branchname`
- `git branch -a`
- `git push origin --delete branchname`