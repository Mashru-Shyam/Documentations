### Setup and Configuration
- git config --global user.name "Your Name"
- git config --gloabal user.email "you@example.com"
- git config --list

### Starting a Project
- git init : Initalize the local git repository
- git clone <url> : Download the project from GitHub

### Workflow with Git
- git status : List of new files and modified files
- git add . : Stage all files for next commit
- git add <filename> : Stage the file for next commit
- git commit -m "Message" : Provide a message for the commit

### Parallel Development
- git branch : List all the branch
- git branch <branch-name> : Create a new branch
- git checkout <branch-name> : Switch to specific branch
- git -b checkout <branch-name> : Create and switch to new branch
- git branch -d <branch-name> : Delete the branch

### Merging
- git merge <branch-name> : Merge the branch to current branch
- git merge --abort : Cancel the merge if conflicts

### Remote Integration
- git remote -v : List all the remote repository linked to the local repository
- git fetch : Download from remote but do not merge
- git pull : Download and merge to current branch
- git push : Upload local commits to remote
- git push -u origin <branch-name> : Pushes a new branch to remote and tracks it

### Undo and Fix
- git log
- git reset --soft Head~1 : Undo last commit but keeps your changes staged
- git reset --haed Head~1 : Undoes latest commit and delete all the changes
- git restore <file-name> : Discarrd local changes to specific files (reverts to last commit)
- git clean -fd : Removes all untracked files and directory

### Temporary Save
- git stash : Temporarily save changes without commiting (clean workspace)
- git stash pop : Restore most recent stash changes
- git stash list

### Advance
- git diff : Show exactly what lines changes
- git blame <filename> : Show who wrote each line of file