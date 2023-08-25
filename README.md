# Git-Command-Guide

This README provides a quick reference for commonly used Git commands. Git is a distributed version control system that helps you manage and track changes to your codebase. Below are the essential Git commands:

## Configuration

Configure your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@example.com"
```

## Repository Creation

Initialize a new repository:

```bash
git init
```

Clone a repository:

```bash
git clone <repository_url>
```

## Basic Workflow

Check the status of your working directory:

```bash
git status
```

Stage changes for commit:

```bash
git add <file_name>      # Stage a specific file
git add .                # Stage all changes
```

Commit staged changes:

```bash
git commit -m "Commit message"
```

## Branching

List all branches:

```bash
git branch -a
```

Create a new branch:

```bash
git branch <branch_name>
```

Switch to a branch:

```bash
git checkout <branch_name>
```

Create and switch to a new branch:

```bash
git checkout -b <new_branch_name>
```

Merge a branch into the current branch:

```bash
git merge <branch_name>
```

Delete a branch (locally):

```bash
git branch -d <branch_name>
```

## Remote Repositories

List remote repositories:

```bash
git remote -v
```

Add a remote repository:

```bash
git remote add <remote_name> <repository_url>
```

Fetch changes from a remote repository:

```bash
git fetch <remote_name>
```

Pull changes from a remote repository into the current branch:

```bash
git pull <remote_name> <branch_name>
```

Push local changes to a remote repository:

```bash
git push <remote_name> <branch_name>
```

## Collaboration

View the commit history:

```bash
git log
```

View a specific file's changes:

```bash
git log -p <file_name>
```

Create a pull request (if using a platform like GitHub):

1. Push your branch to the remote repository.
2. Go to the repository's web page.
3. Click on "New Pull Request" and follow the prompts.

## Undoing Changes

Discard changes in the working directory:

```bash
git checkout -- <file_name>
```

Unstage a file (undo `git add`):

```bash
git reset HEAD <file_name>
```

Amend the last commit:

```bash
git commit --amend
```

## Miscellaneous

Show differences between commits, branches, or files:

```bash
git diff
git diff <commit_hash>
git diff <branch_name>..<other_branch_name>
git diff <file_name>
```

Tag a specific commit:

```bash
git tag <tag_name> <commit_hash>
```

Push tags to remote:

```bash
git push --tags
```

These are some of the most frequently used Git commands. Remember to refer to the official [Git documentation](https://git-scm.com/docs) for more in-depth information about each command.

Happy coding!
