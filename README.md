# Comprehensive Git & GitHub Commands Guide

This repository provides a detailed reference of Git and GitHub commands for modern development workflows. From initial setup to advanced operations, enhance your version control skills with this comprehensive guide.

<div align="center">
    <img src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" alt="Git Logo" width="150px">
</div>

## 📑 Table of Contents
- [Initial Setup](#-initial-setup)
- [Repository Management](#-repository-management)
- [Branching & Merging](#-branching--merging)
- [Remote Operations](#-remote-operations)
- [Collaboration](#-collaboration)
- [Undoing Changes](#-undoing-changes)
- [Stashing](#-stashing)
- [Tags](#-tags)
- [Submodules](#-submodules)
- [Advanced Operations](#-advanced-operations)
- [GitHub Pull Requests](#-github-pull-requests)
- [Tips and Resources](#-tips-and-resources)

## 🚀 Initial Setup

| Command | Description |
|---------|-------------|
| `git init` | Create a new Git repository |
| `git clone <url>` | Download a repository from GitHub |
| `git clone --branch <name> <url>` | Clone a specific branch |
| `git config --global user.name "Name"` | Set global username |
| `git config --global user.email "email"` | Set global email |
| `git config --list` | View all configuration settings |

## 📁 Repository Management

| Command | Description |
|---------|-------------|
| `git status` | Check repository status |
| `git add <file>` | Stage specific files |
| `git add .` | Stage all changes |
| `git add -p` | Stage changes interactively |
| `git commit -m "message"` | Commit staged changes |
| `git commit -a -m "message"` | Stage and commit tracked files |
| `git log` | View commit history |
| `git log --oneline` | View simplified commit history |
| `git log --graph --all` | View branch history graph |
| `git show <commit-hash>` | Show commit details |
| `git diff` | Show unstaged changes |
| `git diff --staged` | Show staged changes |

## 🌿 Branching & Merging

| Command | Description |
|---------|-------------|
| `git branch` | List local branches |
| `git branch -a` | List all branches |
| `git branch <name>` | Create new branch |
| `git checkout <name>` | Switch branches |
| `git checkout -b <name>` | Create and switch to branch |
| `git merge <branch>` | Merge branch into current branch |
| `git rebase <branch>` | Reapply commits on another branch |
| `git branch -d <name>` | Delete merged branch |
| `git branch -D <name>` | Force delete branch |
| `git branch -m <old> <new>` | Rename branch |

## 🌎 Remote Operations

| Command | Description |
|---------|-------------|
| `git remote add origin <url>` | Add remote repository |
| `git remote -v` | List remote repositories |
| `git push origin <branch>` | Upload commits to GitHub |
| `git push --all` | Push all branches |
| `git push --set-upstream origin <branch>` | Set tracking branch |
| `git pull origin <branch>` | Download and merge changes |
| `git fetch origin` | Retrieve updates without merging |
| `git push origin --delete <branch>` | Delete remote branch |

## 👥 Collaboration

| Command | Description |
|---------|-------------|
| `git cherry-pick <commit-hash>` | Apply commit from another branch |
| `git fetch --prune` | Update remote tracking branches |

**Resolving Conflicts:**
1. Edit conflicting files
2. `git add <file>` to mark as resolved
3. `git commit` or `git rebase --continue` to finish

## ↩️ Undoing Changes

| Command | Description |
|---------|-------------|
| `git restore <file>` | Discard changes to file |
| `git restore --staged <file>` | Unstage file |
| `git commit --amend` | Modify last commit |
| `git revert <commit-hash>` | Create commit to undo changes |
| `git reset --soft <commit-hash>` | Reset HEAD keeping changes staged |
| `git reset --hard <commit-hash>` | Reset HEAD discarding changes |
| `git clean -f` | Remove untracked files |
| `git clean -fd` | Remove untracked files and directories |

## 📦 Stashing

| Command | Description |
|---------|-------------|
| `git stash` | Save uncommitted changes |
| `git stash save "message"` | Save with description |
| `git stash list` | List saved stashes |
| `git stash apply` | Apply recent stash |
| `git stash apply stash@{n}` | Apply specific stash |
| `git stash drop stash@{n}` | Delete specific stash |
| `git stash pop` | Apply and remove recent stash |
| `git stash clear` | Delete all stashes |

## 🏷️ Tags

| Command | Description |
|---------|-------------|
| `git tag <name>` | Create lightweight tag |
| `git tag -a <name> -m "message"` | Create annotated tag |
| `git tag` | List all tags |
| `git push origin <tag-name>` | Push specific tag |
| `git push origin --tags` | Push all tags |
| `git tag -d <name>` | Delete local tag |
| `git push origin --delete <name>` | Delete remote tag |

## 🧩 Submodules

| Command | Description |
|---------|-------------|
| `git submodule add <url>` | Add repository as submodule |
| `git submodule init` | Initialize submodules |
| `git submodule update` | Update submodules |
| `git submodule update --remote` | Update to latest commits |
| `git clone --recurse-submodules <url>` | Clone with submodules |

## ⚙️ Advanced Operations

| Command | Description |
|---------|-------------|
| `git rebase -i <commit-hash>` | Interactive rebase |
| `git bisect start` | Begin binary search for bugs |
| `git bisect bad` | Mark current commit as bad |
| `git bisect good <commit-hash>` | Mark commit as good |
| `git bisect reset` | End bisect session |
| `git log --follow <file>` | Show file history |
| `git blame <file>` | Show who modified each line |
| `git log -S "term"` | Search commits for term |
| `git format-patch -1 <commit-hash>` | Generate patch file |
| `git apply <patch-file>` | Apply patch |

## 🔄 GitHub Pull Requests

**Creating a Pull Request:**
1. Push your branch to GitHub
2. Navigate to repository on GitHub
3. Select your branch and click "New Pull Request"
4. Add title, description, and submit

**Syncing a Fork:**
```bash
git remote add upstream <original-url>
git fetch upstream
git merge upstream/main
git push origin main
```

## 💡 Tips and Resources

- Write clear, descriptive commit messages
- Pull before pushing to avoid conflicts
- Use branches for features and bug fixes
- Be careful with history-rewriting commands

**Learn More:**
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com/en)
- [Pro Git Book](https://git-scm.com/book/en/v2)

<div align="center">
    <p>Happy version controlling!</p>
</div>
