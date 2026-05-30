# Git for beginners

A documentation/cheatsheet of Git for myself.

## Git workflow

1. Modify files
2. git add <file>
3. git commit -m "message"
4. git push

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
  Restore a file to the last commit

- `git commit -m "message"`  
  Commit with a message

- `git status`  
  Show repository status and changed files

- `git log`  `git log --oneline --graph --all`  
  Show commit history

- `git diff`  
  Shows changes not yet committed

- `git diff --staged`  
  Shows staged changes that will be included in the next commit

- `git show`
  Show details of the latest commit

## Branch commands

- `git branch`  
  Shows all local branches and highlights the current branch

- `git switch <branch/commit> (-c branch_name)`  
  Switches active branch or creates with -c

- `git merge <branch>`  
  Merges the specified branch into the currently active branch

- `git branch -d <branch>`  
  Delete branch

## GitHub commands

- `git remote add <name> <url>`  
  Connect local repository to github

- `git push -u <remote> <branch>`
  Pushes a branch and sets the upstream tracking branch.
  After the first push, `git push` is usually enough.

- `git remote -v`  
  Check where repository is connected

- `git clone <url>`  
  Clones the repository to the current working directory

- `git clone <url> my-project`  
  Clones into a folder named my-project

- `git pull`  
  Pulls the latest changes

- `git fetch`
  Download changes from remote without merging them