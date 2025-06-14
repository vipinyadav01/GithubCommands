# GitHub Commands for Beginners

A modern guide to essential GitHub commands for new users.

## Getting Started

### Setting Up Git

```bash
# Configure your identity
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Check your configuration
git config --list
```

### Creating a Repository

```bash
# Initialize a new repository
git init

# Clone an existing repository
git clone https://github.com/username/repository.git
```

## Basic Workflow

### Tracking Changes

```bash
# Check status of your files
git status

# Add files to staging area
git add filename.txt    # Add specific file
git add .               # Add all files

# Commit your changes
git commit -m "Your commit message"
```

### Working with Remote Repositories

```bash
# Connect to a remote repository
git remote add origin https://github.com/username/repository.git

# Push changes to GitHub
git push -u origin main    # First time push
git push                   # Subsequent pushes

# Get updates from GitHub
git pull
```

## Branching

```bash
# Create a new branch
git branch branch-name

# Switch to a branch
git checkout branch-name

# Create and switch to a new branch
git checkout -b branch-name

# Merge a branch into current branch
git merge branch-name

# Delete a branch
git branch -d branch-name
```

## Additional Useful Commands

```bash
# View commit history
git log
git log --oneline --graph

# Undo changes before staging
git checkout -- filename.txt

# Undo staged changes
git reset HEAD filename.txt

# Create a tag
git tag v1.0.0
```

## GitHub-Specific Features

- **Pull Requests**: Propose changes through the GitHub interface
- **Issues**: Track bugs and feature requests
- **Actions**: Automate workflows
- **Projects**: Manage tasks and workflows

## Visual GitHub Clients

If you prefer a graphical interface:
- GitHub Desktop
- Visual Studio Code with Git extensions
- GitKraken

Happy coding! 🚀