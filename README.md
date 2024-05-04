# Git Commands

_A list of commonly used Git commands._

**Note**: The following commands assume that you have Git installed and have basic knowledge of using the command line interface. {Usman Ghias}

## Table of Contents

- [Getting & Creating Projects](#getting--creating-projects)
- [Basic Snapshotting](#basic-snapshotting)
- [Branching & Merging](#branching--merging)
- [Sharing & Updating Projects](#sharing--updating-projects)
- [Inspection & Comparison](#inspection--comparison)

## Getting & Creating Projects

To start using Git for version control in your projects, follow these commands:

```bash
# Initialize a local Git repository
git init

# Create a local copy of a remote repository
git clone ssh://git@github.com/[username]/[repository-name].git
```

## Basic Snapshotting

These commands help you manage and track changes in your project:

```bash
# Check status
git status

# Add a file to the staging area
git add [file-name.txt]

# Add all new and changed files to the staging area
git add -A

# Commit changes
git commit -m "[commit message]"

# Remove a file (or folder)
git rm -r [file-name.txt]
```

## Branching & Merging

Git provides powerful branching and merging capabilities:

```bash
# List branches (the asterisk denotes the current branch)
git branch

# List all branches (local and remote)
git branch -a

# Create a new branch
git branch [branch name]

# Delete a branch
git branch -d [branch name]

# Delete a remote branch
git push origin --delete [branch name]

# Create a new branch and switch to it
git checkout -b [branch name]

# Clone a remote branch and switch to it
git checkout -b [branch name] origin/[branch name]

# Rename a local branch
git branch -m [old branch name] [new branch name]

# Switch to a branch
git checkout [branch name]

# Switch to the branch last checked out
git checkout -

# Discard changes to a file
git checkout -- [file-name.txt]

# Merge a branch into the active branch
git merge [branch name]

# Merge a branch into a target branch
git merge [source branch] [target branch]

# Stash changes in a dirty working directory
git stash

# Remove all stashed entries
git stash clear
```

## Sharing & Updating Projects

These commands help you share your changes and update your local repository:

```bash
# Push a branch to your remote repository
git push origin [branch name]

# Push changes to remote repository (and remember the branch)
git push -u origin [branch name]

# Push changes to remote repository (remembered branch)
git push

# Delete a remote branch
git push origin --delete [branch name]

# Update local repository to the newest commit
git pull

# Pull changes from remote repository
git pull origin [branch name]

# Add a remote repository
git remote add origin ssh://git@github.com/[username]/[repository-name].git

# Set a repository's origin branch to SSH
git remote set-url origin ssh://git@github.com/[username]/[repository-name].git
```

## Inspection & Comparison

To inspect and compare changes in your project, use these commands:

```bash
# View changes
git log

# View changes (detailed)
git log --summary

# View changes (

briefly)
git log --oneline

# Preview changes before merging
git diff [source branch] [target branch]
```

## Additional Git Commands

Here are some more commonly used Git commands:

```bash
git config
git init
git clone
git add
git commit
git diff
git reset
git status
git rm
git log
git show
git tag
git branch
git checkout
git merge
git remote
git push
git pull
git stash
```


# Configuration & Setup
```bash
# Configure user name globally
git config --global user.name "Usman Ghias"

# List all configurations
git config --list

# Set SSH for GitHub
git remote set-url origin git@github.com:[username]/[repository-name].git
```
# Advanced Usage
```bash
# Visualize branch topology
git log --all --graph

# Revert file to a previous commit
git checkout [commit-hash] [file-name.txt]

# Reset current HEAD to a specified state
git reset --hard [commit-hash]

# Modify commit messages
git commit --amend -m "New message"

# List all stashed changes
git stash list
```

Feel free to explore and use these commands to effectively manage your Git repositories. {Usman Ghias}
[CODCrafters](https://www.codcrafters.org/contactus)
Please refer to the [official Git documentation](https://git-scm.com/doc) for more information and advanced usage of Git commands.
