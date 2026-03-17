Here’s a simple **Git & GitHub command** you can copy directly.

# Git & GitHub Command Cheat Sheet

## 1. Configure Git (First Time Setup)

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
````

Check configuration:

```bash
git config --list
```

---

# 2. Initialize Repository

Create a new git repository:

```bash
git init
```

---

# 3. Clone Repository

Clone an existing GitHub repository:

```bash
git clone https://github.com/username/repository.git
```

---

# 4. Check Repository Status

```bash
git status
```

---

# 5. Add Files to Staging

Add a specific file:

```bash
git add filename
```

Add all files:

```bash
git add .
```

---

# 6. Commit Changes

```bash
git commit -m "Your commit message"
```

---

# 7. Connect to GitHub Repository

```bash
git remote add origin https://github.com/username/repository.git
```

Check remote:

```bash
git remote -v
```

---

# 8. Push Code to GitHub

First push:

```bash
git push -u origin main
```

Normal push:

```bash
git push
```

---

# 9. Pull Latest Changes

```bash
git pull origin main
```

---

# 10. Branch Commands

Create new branch:

```bash
git branch branch-name
```

Switch branch:

```bash
git checkout branch-name
```

Create & switch:

```bash
git checkout -b branch-name
```

List branches:

```bash
git branch
```

Delete branch:

```bash
git branch -d branch-name
```

---

# 11. Merge Branch

```bash
git merge branch-name
```

---

# 12. View Commit History

```bash
git log
```

Short log:

```bash
git log --oneline
```

---

# 13. Undo Changes

Unstage file:

```bash
git reset filename
```

Discard changes:

```bash
git checkout -- filename
```

---

# 14. Remove File

```bash
git rm filename
```

---

# 15. Update Local Repo

```bash
git fetch
git pull
```

---
Here is a **typical Git & GitHub workflow format** 

# Git & GitHub Workflow

## 1. Clone the Repository

Download the project from GitHub to your local machine.

```bash
git clone https://github.com/username/repository.git
cd repository
```

---

## 2. Create a New Branch

Always create a branch for new features or fixes.

```bash
git checkout -b feature-branch
```

---

## 3. Make Changes

Edit or create files in the project.

Check status:

```bash
git status
```

---

## 4. Add Files to Staging

Stage the files you want to commit.

```bash
git add .
```

Or add a specific file:

```bash
git add filename
```

---

## 5. Commit Changes

Save the staged changes with a message.

```bash
git commit -m "Add new feature"
```

---

## 6. Push Branch to GitHub

Upload your branch to GitHub.

```bash
git push origin feature-branch
```

---

## 7. Create Pull Request (PR)

1. Go to the repository on GitHub.
2. Click **Compare & Pull Request**.
3. Add description.
4. Submit the Pull Request.

---

## 8. Review & Merge

After review:

* Fix issues if requested.
* Merge the Pull Request into `main`.

---

## 9. Update Local Repository

After merging, update your local repository.

```bash
git checkout main
git pull origin main
```

---

## 10. Delete Branch

Delete the branch after merging.

```bash
git branch -d feature-branch
git push origin --delete feature-branch
```

---

# Simple Workflow Summary

```text
Clone Repo
   ↓
Create Branch
   ↓
Make Changes
   ↓
Add → Commit
   ↓
Push Branch
   ↓
Create Pull Request
   ↓
Review & Merge
   ↓
Pull Latest Code
```

---

# Best Practices

* Create **small commits**.
* Write **clear commit messages**.
* Always **pull latest code before pushing**.
* Use **branches for every feature or bug fix**.

# Useful Tips

* `main` is the default branch in most GitHub repositories.
* Always `git pull` before `git push`.
* Write meaningful commit messages.

```
