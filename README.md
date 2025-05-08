## Git Branching Practice

### Basic Commands
* `git init`  - initialize local git repo in current folder (working deirectory)
* `git add .` - stage all changes for commit
* `git commit -m "message"` - commit staged changes to local repo

### Info Commands
* `git status` - show current status of working directory
* `git log` - show local commit history
* `git log --oneline` - showe lcoal commit history, compact format

* `git config -l` - list configuration of local repo

* `git config -- global -l` - list global configuration
* `git version` - show version of installed git

### Branching Commands
* `git branch` - list local branches
* `git branch branchName` - create new bracnch  `branchName`
* `git checkout branchName` - switch to new bracnch  `branchName`

### Remote Commands
* `git remote add alias URL` - connect local repo ro remote, using name `alias` for remote repo `URL`
* `git push alias branchName` - push local commits to rmeote repo `alisa` on branch `branchName`

### Git Branch Workflow
1. Go to local `main` branch
	`git checkout main`
2. Pull remote main
	`git pull origin main`
3. Create and check out a new branch
	`git checkout -b featureName`
4. Work on your branch, committing frequently
5. When task complete, pull main and fix merge conflicts
	`git add .
	 git commit -m "Complete Feature"
	 git pull origin main`

	 Fix any merge conflicts and commit the fix.
 6. Push to your branch
 	`git push origin featureName`
7. Create pull request on GitHub
8. Merge pull request to main
