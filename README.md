# Git Branching

## Basic Commands
* `git init` - initialize local git repository
* `git add .` - stage files in working directory for commit
* `git commit -m "message"` - commit stages files with commit message `message`

## Info Commands
* `git status` - show stage of local working directory
* `git log` - list commit history
* `git log --online` - list commit history, compact format
* `git config -l` - list locatl git configuration

## Branching Commands
* `git branch` - list local branches
* `git branch branchName` - create local branch `branchName`
* `git checkout branchName` - move to branch

## Remote Commands
* `git remove add origin URL` - set `origin` as alias for remote repo `URL`
* `git push origin branchName` - push local commits to `origin` repo on branch `branchName`