# Git for beginners

A documentation of Git for myself.

## Basic commands

- `git --version`  
  Shows the currently installed Git version.

- `git init`  
  Initializes Git in the current directory.

- `git config --global user.name "Name"`  
  Sets the name that will appear on commits.

- `git config --global user.email "Email"`  
  Sets the mail that will appear on commits.

- `git add <file/dir> (. for everything)`  
  Add files/directories to staging for the next commit

- `git restore --staged file.txt`  
  Remove a file from staging

- `git restore file.txt`  
  Restor a file to the last commit

- `git commit -m "message"`  
  Commit with a message

- `git status`  
  Show repository status and changed files

- `git log`  `git log --oneline --graph --all`  
  Show commit history

- `git diff (--staged)`  
  Shows changes not yet committed

## Branch commands

- `git branch`  
  Shows current branch and active branches

- `git switch <branch/commit> (-c branch_name)`  
  Switches active branch or creates with -c

- `git merge <branch>`  
  Branch to merge to the currently active branch

- `git branch -d <branch>`  
  Delete branch

## GitHub commands

- `git remote add <name> <url>`  
  Connect local repository to github

- `git push (-u <name> <branch>)`  
  Pushes the branch to github (-u and arguments for first time only)

- `git remote -v`  
  Check where repository is connected

- `git clone <url>`  
  Clones the repository to the current working directory

- `git pull`  
  Pulls the latest changes