# Git and GitHub Commands for Terminal Users

## Beginner Commands

### Setup

```bash
# Configure your identity
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Initialize a repository
git init
```

### Basic Workflow

```bash
# Check status
git status

# Add files to staging area
git add filename.txt    # Add specific file
git add .               # Add all files

# Commit changes
git commit -m "Your commit message"

# View commit history
git log
```

### Remote Repositories

```bash
# Clone a repository
git clone https://github.com/username/repository.git

# Connect to a remote repository
git remote add origin https://github.com/username/repository.git

# Push to GitHub
git push -u origin main

# Pull from GitHub
git pull origin main
```

## Intermediate Commands

### Branching

```bash
# Create a new branch
git branch branch-name

# Switch to a branch
git checkout branch-name

# Create and switch in one command
git checkout -b branch-name

# List all branches
git branch -a

# Merge a branch
git merge branch-name
```

### Advanced Operations

```bash
# Stash changes
git stash
git stash pop

# Check differences
git diff
git diff --staged

# Undo last commit but keep changes
git reset --soft HEAD~1

# Discard local changes
git checkout -- filename.txt

# Discard all local changes
git reset --hard

# Amend last commit
git commit --amend
```

### Collaboration

```bash
# Fetch updates without merging
git fetch origin

# Create a pull request (GitHub CLI)
gh pr create --base main --head feature-branch

# Review pull requests (GitHub CLI)
gh pr list
gh pr checkout PR_NUMBER
```

### Tag Management

```bash
# Create a tag
git tag v1.0.0

# Create an annotated tag
git tag -a v1.0.0 -m "Version 1.0.0"

# Push tags
git push origin --tags
```

### Troubleshooting

```bash
# View commit history with graph
git log --graph --oneline --all

# Find which commit introduced a bug
git bisect start
git bisect bad    # Current version is bad
git bisect good v1.0.0    # v1.0.0 was good

# Rebase branches
git rebase main
```