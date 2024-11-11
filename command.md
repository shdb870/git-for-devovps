Git Command Reference
This document provides an overview of commonly used Git commands.

Basic Git Commands
git init
Initializes a new Git repository in the current directory.
Example: git init
git clone <repository>
Creates a copy of an existing Git repository.
Example: git clone https://github.com/user/repo.git
git status
Displays the current status of the repository, showing changes that are staged, unstaged, and untracked files.
Example: git status
git add <file>
Adds changes in the specified file to the staging area.
Example: git add filename.txt
git commit -m "<message>"
Commits the changes in the staging area with a descriptive message.
Example: git commit -m "Initial commit"
git push <remote> <branch>
Pushes commits to a remote repository on the specified branch.
Example: git push origin main
git pull <remote> <branch>
Fetches changes from a remote repository and merges them into the current branch.
Example: git pull origin main
git fetch
Fetches changes from a remote repository without merging them.
Example: git fetch
git log
Displays the commit history for the repository.
Example: git log
git diff
Shows the differences between the working directory and the staging area, or between commits.
Example: git diff
Working with Branches
git branch
Lists all local branches in the current repository.
Example: git branch
git branch <branch-name>
Creates a new branch with the given name.
Example: git branch feature-branch
git checkout <branch-name>
Switches to the specified branch.
Example: git checkout feature-branch
git checkout -b <branch-name>
Creates a new branch and immediately switches to it.
Example: git checkout -b new-branch
git merge <branch-name>
Merges the specified branch into the current branch.
Example: git merge feature-branch
git rebase <branch-name>
Reapplies commits from the current branch onto another branch, effectively replaying the changes.
Example: git rebase main
Git Staging and Unstaging
git add <file>
Adds a specific file to the staging area.
Example: git add filename.txt
git reset <file>
Removes a file from the staging area, without changing the file content.
Example: git reset filename.txt
git reset --hard
Resets the working directory and staging area to match the most recent commit. Warning: This will discard any changes.
Example: git reset --hard
Git Undo
git restore <file>
Discards changes in the specified file and restores it to the state of the last commit.
Example: git restore filename.txt
git revert <commit>
Reverts a commit by creating a new commit that undoes the changes of a previous commit.
Example: git revert 1a2b3c4d
Remote Repositories
git remote add <name> <url>
Adds a remote repository to your local repository.
Example: git remote add origin https://github.com/user/repo.git
git remote -v
Displays the URLs of the remotes associated with the repository.
Example: git remote -v
git remote remove <name>
Removes a remote repository from your local repository.
Example: git remote remove origin
Advanced Git Commands
git tag <tag-name>
Creates a tag at the current commit.
Example: git tag v1.0
git stash
Stashes changes (both staged and unstaged) to be applied later.
Example: git stash
git stash pop
Applies the most recent stash and removes it from the stash list.
Example: git stash pop
Git Configuration
git config --global user.name "<name>"
Sets the global user name for commits.
Example: git config --global user.name "John Doe"
git config --global user.email "<email>"
Sets the global user email for commits.
Example: git config --global user.email "john.doe@example.com"
git config --list
Displays all Git configuration settings.
Example: git config --list
Other Useful Commands
git rm <file>
Removes a file from both the working directory and the staging area.
Example: git rm filename.txt
git clean -f
Removes untracked files from the working directory.
Example: git clean -f
git show <commit>
Shows details about a specific commit.
Example: git show 1a2b3c4d
git help <command>
Displays help information about a specific Git command.
Example: git help commit
