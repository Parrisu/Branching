# Git Branching


## Overview

Summary of common git commands, and practice with branching.

## Summary of Branch Workflow

1. Checkout and pull main

	```bash
	git checkout main
	git pull origin main
	```
2. Checkout new branch from up-to-date main
	```bash
	git checkout -b someFeature
	```
3. Work, committing each ocmpleted task, until feature is ocmplete
4. Pull remote main into local branch
	```bash
	git add .
	git commit -m "Complete feature"
	git pull origin main
	```

		* if auto merge succeeds, save and quit from `vi` editor:
		```
		:wq
		```
		* if `CONFLICT`, fix conflicts in all files removing merge markers and commit
		```bash
		git add .
		git commit -m "Fix merge conflicts"
		```
5. Push to remote branch
	```bash
	git push origin someFeature
	```
6. On Github, create pull request and merge with main.
7. Checkout and pull merged main.
	```bash
	git checkout main
	git pull origin main
	```



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
* `git pull origin branchName` - pull remote branch `branchName` into current local branch

<<<<<<< HEAD
 
=======
<<<<<<< HEAD

# Main
=======
# Testing
>>>>>>> refs/remotes/origin/main
>>>>>>> 764c29e3e5909dfb56452b8ec06026a94af72df5
