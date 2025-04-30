# Git Cheatsheet

## Introduction
Git is a version control system that tracks changes to your files over time. This cheatsheet provides a simple explanation of Git concepts and common commands to help you get started with version control.

## What is Git?
Git is like a history book for your project. It keeps track of every change you make to your files over time, allowing you to:
- Go back to older versions when needed
- Collaborate with others without overwriting each other's work
- Track changes (what was changed, when, and by whom)
- Experiment safely with new features in branches

## Key Git Concepts

### Repository (Repo)
The main folder for your project that Git tracks, containing all files and change history.

### Working Directory
Your local folder where you edit project files and make changes.

### Staging Area (Index)
A temporary area where you prepare changes before committing them. Think of it as a "waiting room" for your changes.

### Commit
A snapshot of your project at a specific point in time, like saving a version of your work. Each commit includes a message describing the changes.

### Branch
A separate timeline of development where you can work on features or fixes without affecting the main codebase. The main branch is typically called `main` or `master`.

### Remote Repository
A repository hosted on a server (like GitHub, GitLab, or Bitbucket) where you can share code and collaborate with others.

## Common Git Commands

### Basic Setup & Info

| Command | Description | Example |
|---------|-------------|---------|
| `git config --global user.name "Your Name"` | Sets your name for commits (globally) | `git config --global user.name "John Doe"` |
| `git config --global user.email "email@example.com"` | Sets your email for commits (globally) | `git config --global user.email "john@email.com"` |
| `git init` | Initializes a new Git repository | `git init` |
| `git clone <repository_url>` | Downloads a repository from a remote URL | `git clone https://github.com/user/repo.git` |
| `git status` | Shows the status of your working directory | `git status` |

### Working with Changes

| Command | Description | Example |
|---------|-------------|---------|
| `git add <filename>` or `git add .` | Stages changes in specific or all files | `git add index.html` or `git add .` |
| `git commit -m "Your commit message"` | Commits staged changes with a message | `git commit -m "Fixing a bug in login form"` |
| `git diff` | Shows differences between working directory and staging area | `git diff` |
| `git diff --staged` | Shows differences between staging area and last commit | `git diff --staged` |
| `git restore --staged <filename>` | Unstages a file | `git restore --staged index.html` |
| `git restore <filename>` | Discards changes in working directory | `git restore index.html` |

### Viewing History

| Command | Description | Example |
|---------|-------------|---------|
| `git log` | Shows commit history | `git log` |
| `git log --oneline` | Shows condensed one-line commit history | `git log --oneline` |
| `git show <commit_hash>` | Shows details of a specific commit | `git show a1b2c3d4` |

### Branching

| Command | Description | Example |
|---------|-------------|---------|
| `git branch` | Lists all branches (current highlighted) | `git branch` |
| `git branch <branch_name>` | Creates a new branch | `git branch feature-login` |
| `git checkout <branch_name>` | Switches to a different branch | `git checkout feature-login` |
| `git checkout -b <new_branch_name>` | Creates and switches to a new branch | `git checkout -b develop` |
| `git merge <branch_name>` | Merges changes from specified branch into current | `git merge develop` |
| `git branch -d <branch_name>` | Deletes a branch (after it's merged) | `git branch -d feature-login` |

### Remote Repositories

| Command | Description | Example |
|---------|-------------|---------|
| `git remote add origin <repository_url>` | Adds a remote repository named "origin" | `git remote add origin https://github.com/user/repo.git` |
| `git remote -v` | Shows configured remote repositories | `git remote -v` |
| `git push origin <branch_name>` | Uploads local commits to remote | `git push origin main` |
| `git pull origin <branch_name>` | Downloads changes from remote to local | `git pull origin main` |
| `git fetch origin` | Downloads objects and refs from remote | `git fetch origin` |

## Key Command Explanations

- **git init**: Start using Git in your project folder
- **git clone**: Download an existing Git project
- **git add**: Stage files for the next commit
- **git commit**: Save a snapshot of staged changes
- **git status**: Check what's happening in your repository
- **git branch** and **git checkout**: Work with different development branches
- **git push**: Send local commits to a remote repository
- **git pull**: Get and merge latest changes from remote repository

## Best Practices

1. **Commit Frequently**: Make smaller, logical commits instead of large ones
2. **Write Good Commit Messages**: Explain why you made changes, not just what changed
3. **Use Branches**: Create branches for new features or bug fixes

## Git Interview Questions

1. What is Git and why is it important in software development?
2. Explain the difference between `git add`, `git commit`, and `git push`
3. What is a branch in Git and why are branches useful?
4. How do you merge changes from one branch to another in Git?
5. What is a remote repository and why do we use them?
6. Describe a typical Git workflow for developing a new feature
7. What is a merge conflict and how do you resolve it?

---
*This is a starting point for Git. There's much more to learn, but these basics and commands will get you going! Practice using these commands in a test repository to get comfortable with Git.*
