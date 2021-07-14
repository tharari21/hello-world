# hello-world

## Configuring

**git config --global user.name "your_name"**
**git config --global user.email "your_email"**
**git config --global color.ui auto** - enables command line coloring output
**git config** - get different config options
**git config --list** or **git config -l** press q to exit
**git init .** - initializes git repository - adds a folder named .git that contains everything needed
Only use git init for brand new projects not if project exists
**rm -rf .git** - delete git folder - un-init's the directory

## Staging Files

**git status** - Gives us status of changes we have made
**git add <filename>** - Stage specific files in dir
**git add .** - Stage all files in current dir
**git add -A** - Stage all files in current dir and all sub dirs
**git rm -r --cached .** - Unstage all files in dir
**git rm --cached <filename>** - unstage files

## Commit Files

**git commit -m "Commit Message"**
**git log** - See the commit history - gives hash,authod,date...
To see the actual changes of the commit, copy the hash of the commit and run the following:
**git show <hash>** - q to exit
**git diff** - Shows diff btwn what you have in cwd and what has been commited
**git restore <filename>** - undo to last commit
**git commit --amend -m "Your message"** - Allows you to amend the last commit message

## Pushing Files

**git remote add origin <url>** - connect local direcory to remote git project
**git branch -M main** - change from master to main
**git push -u origin main** - if you get fatal: Could not read remote repository error then you need to configure ssh - go to github help page on this topic where they guide step by step
the -u origin main only needs to be done once - every other time you can just say git push

## Pull Files
**git pull** - Bring latest changes from remote repo

## Branches
**git branch** - Lists local branches
**git branch -r** - List remote branches
**git branch -a** - List all branches local and remote - branches starting with remotes/origin are remote
**git branch <branchname>** - Create new branch (a branch is a copy of the main branch)
**git checkout <branchname>** - Switch to branchname
**git checkout -** - Switch to previous branch you were on