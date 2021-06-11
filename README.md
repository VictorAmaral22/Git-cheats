# Git Cheats
![1f265e2d4c43](https://user-images.githubusercontent.com/47861954/120095491-ae178280-c0fc-11eb-8ad5-d5afb0ba50c8.png)
## Configuring
Configs your username
```
git config --global user.name "Fulaninho.yelss"
```

Configs your email
```
git config --global user.email "meu.email@gmail.com"
```


## Initializing

Starts a new repository
```
git init
```

It says it all
```
git add README.md
```

Clones a repository from github
```
git clone http://www.github.com/clebinho.pneu/exemple-repo
```

Adds a online repository as the repo you will push your files to
```
git remote add origin https://github.com/clebinho.pneu/Tutorial.git
```


## After the changes

Adds all the modified files to your commit
```
git add .
```

Cancels the 'git add'
```
git restore --staged .
```

Prepares the files that you will send and attaches a message from the committer with them, describing what was changed.
```
git commit -m "Lorem impsum"
```

Pushes the commit for the repository
```
git push -u origin master
```


## Managing branches

Creates a new branch called 'newBranch'
```
git checkout -b newBranch
```

Returns to the master branch
```
git checkout master
```

Removes the 'newBranch'
```
git branch -d newBranch
```


## Updating your repo

This makes your offline repo updated with the online repo
```
git pull
```

This merges the active branch with the one called on the function
```
git merge <branch>
```


## Useful things

If you did something wrong, it will retun to the latest change in the HEAD
```
git checkout -- <archive>
```

This is usefull if you want to cancel the local changes and commits
```
git fetch origin
git reset --hard origin/master
```

Removes the remote origin obviously
```
git remote remove origin
```


## Checking if everything's all right

Shows you how is the working tree
```
git status
```

List all the latest commits
```
git log
```

Shows you the remote origins, like the github repository you set for this project
```
git remote -v
```
