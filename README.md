# Git for beginners

A documentation/cheatsheet of Git for myself.

## Git workflow

0. `git pull` (optional, before starting work)
1. Modify files
2. `git add <file>`
3. `git commit -m "message"`
4. `git push`

## Ignore files

- `.gitignore`
  Lists files and folders Git should ignore.
  Useful for node_modules, logs, build files, etc.

## Basic commands

- `git --version`  
  Shows the currently installed Git version

- `git init`  
  Initializes Git in the current directory

- `git config --global user.name "Name"`  
  Sets the name that will appear on commits

- `git config --global user.email "Email"`  
  Sets the email address that will appear on commits

- `git add <file/dir> (. for everything)`  
  Adds files/directories to the staging area for the next commit

- `git restore --staged file.txt`  
  Removes a file from the staging area

- `git diff`  
  Shows changes not yet committed or staged

- `git diff --staged`  
  Shows staged changes that will be included in the next commit

- `git commit -m "message"`  
  Commit with a message

- `git status`  
  Show repository status and changed files

- `git restore file.txt`  
  Restores a file to its state in the last commit

- `git log`  
  Show commit history

- `git log --oneline --graph --all`  
  Show compact commit history with branch graph

- `git show`  
  Show details of the latest commit

- `git reset --soft HEAD~1`  
  Undo the last commit but keep the changes. Useful when you commit too early

## Branch commands

- `git branch`  
  Shows all local branches and highlights the current branch

- `git switch <branch>`  
  Switch to an existing branch

- `git switch -c <branch>`  
  Create and switch to a new branch

- `git merge <branch>`  
  Merges the specified branch into the currently active branch

- `git branch -d <branch>`  
  Delete branch

- `git branch -m <name>`  
  Rename currently active branch

- `git stash`  
  Temporarily saves unfinished work without committing it.  
  Useful when switching branches before your work is finished

- `git stash pop`  
  Restores the stashed changes and removes them from the stash

## GitHub commands

- `git remote add <remote> <url>`  
  Connects the local repository to GitHub  
(The remote name can be anything, but "origin" is the standard convention)

- `git push -u <remote> <branch>`
  Pushes a branch and sets the upstream tracking branch.  
  After the first push, `git push` is usually enough.

- `git remote`  
  Shows the names of the remote repositories

- `git remote -v`  
  Shows the configured remote repositories

- `git clone <url>`  
  Clones the repository to the current working directory

- `git clone <url> my-project`  
  Clones into a folder named my-project

- `git pull`  
  Fetches changes from the remote repository and merges them into the current branch.  
  May require resolving merge conflicts if the same files were changed.

- `git fetch`  
  Downloads changes from the remote repository without merging them

- `git merge`  
  Merges the fetched changes.  
  May require resolving merge conflicts if the same files were changed.