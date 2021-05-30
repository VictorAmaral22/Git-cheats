# Git Cheats


## Configuring

```
git config --global user.name "Bruno.Orlandi"
```
Configs your username

```
git config --global user.email "meu.email@gmail.com"
```
Configs your email


## Initializing

```
git init
```
Starts a new repository

```
git add README.md
```
It says it all

```
git clone http://www.github.com/clebinho.pneu/exemple-repo
```
Clones a repository from github

```
git remote add origin https://github.com/clebinho.pneu/Tutorial.git
```
Adds a online repository as the repo you will push your files to


## After the changes

```
git add .
```
Adds all the modified files to your commit

```
git restore --staged .
```
Cancels the 'git add'

```
git commit -m "Lorem impsum"
```
Prepares the files that you will send and attaches a message from the committer with them, describing what was changed.

```
git push -u origin master
```
Pushes the commit for the repository


## Managing branches

```
git checkout -b newBranch
```
Creates a new branch called 'newBranch'

```
git checkout master
```
Returns to the master branch

```
git branch -d newBranch
```
Removes the 'newBranch'


## Updating your repo

```
git pull
```
This makes your offline repo updated with the online repo

```
git merge <branch>
```
This merges the active branch with the one called on the function


## Useful things

```
git checkout -- <archive>
```
If you did something wrong, it will retun to the latest change in the HEAD

```
git fetch origin
git reset --hard origin/master
```
This is usefull if you want to cancel the local changes and commits

```
git remote remove origin
```
Removes the remote origin obviously


## Checking if everything's all right

```
git status
```
Shows you how is the working tree

```
git log
```
List all the latest commits

```
git remote -v
```
Shows you the remote origins, like the github repository you set for this project
