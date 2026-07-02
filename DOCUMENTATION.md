# Day 3 - Git Basics

**Date:** 01 July 2026

---

## 1. Repository Setup

### `git init`
Creates a new empty Git repository in the current folder.

```bash
git init
```

### `git clone`
Copies an existing repository from GitHub to your local system.

```bash
git clone <repository-url>
```

### `git config`
Sets Git username and email.

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

---

## 2. Checking Project Status

### `git status`
Shows the current state of your working directory.

```bash
git status
```

### `git log`
Displays the commit history of the repository.

```bash
git log
```

---

## 3. Saving Changes

### `git add`
Adds files to the staging area.

```bash
git add filename
git add .
```

- `git add filename` → Adds a specific file.
- `git add .` → Adds all changed files.

### `git commit`
Saves staged changes permanently in the local repository.

```bash
git commit -m "Your commit message"
```

---

## 4. Remote Repository Management

### `git remote`
Shows or manages connections to remote repositories.

```bash
git remote -v
```

### `git push`
Uploads local commits to GitHub.

```bash
git push origin main
```

### `git pull`
Downloads and merges changes from GitHub.

```bash
git pull origin main
```

### `git fetch`
Downloads latest changes from GitHub without merging.

```bash
git fetch
```

---

## 5. Branching

### `git branch`
Creates or lists branches.

```bash
git branch
git branch feature-branch
```

### `git checkout`
Switches branches or restores files.

```bash
git checkout feature-branch
```

### `git switch`
Modern command used only for switching branches.

```bash
git switch feature-branch
```

---

## 6. Advanced Git Commands

### `git merge`
Combines changes from one branch into another.

```bash
git merge feature-branch
```

### `git rebase`
Moves commits on top of another branch to maintain a clean history.

```bash
git rebase main
```

### `git cherry-pick`
Copies a specific commit from another branch.

```bash
git cherry-pick <commit-id>
```

---

## 7. Undoing Changes

### `git stash`
Temporarily saves uncommitted changes.

```bash
git stash
```

### `git reset`
Unstages files or removes commits.

```bash
git reset HEAD filename
```

### `git revert`
Creates a new commit that undoes a previous commit.

```bash
git revert <commit-id>
```

---

# Important Comparisons

## `git status` vs `git log`

| Command | Purpose |
|---------|---------|
| `git status` | Shows current changes in the project |
| `git log` | Shows commit history |

---

## `git init` vs `git clone`

| Command | Purpose |
|---------|---------|
| `git init` | Creates a new empty repository |
| `git clone` | Copies an existing repository |

---

## `git checkout` vs `git switch`

| Command | Purpose |
|---------|---------|
| `git checkout` | Switches branches and restores files |
| `git switch` | Only switches branches |

---

# Git Fork (Concept)

A **Fork** creates your own copy of someone else's GitHub repository.

### Uses of Fork
- Contribute to open-source projects.
- Make changes without affecting the original repository.
- Send changes back using a Pull Request.

---

# Key Takeaways

- Git tracks changes in your project.
- GitHub stores your code online.
- Branches allow parallel development.
- `git push` uploads code to GitHub.
- `git pull` downloads code from GitHub.
- `git rebase` helps maintain a clean commit history.
