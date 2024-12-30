# Git Cheat Sheet

## **Git Basics**

### Configure Git (Global)
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

### Initialize a Repository
```bash
git init
```

### Clone a Repository
```bash
git clone <repository_url>
```

### Check Repository Status
```bash
git status
```

### Stage Files
```bash
git add <file>         # Stage a specific file
git add .              # Stage all files
```

### Commit Changes
```bash
git commit -m "Commit message"
```

### View Commit History
```bash
git log
```

---

## **Branching**

### List Branches
```bash
git branch              # Local branches
git branch -a           # All branches (local + remote)
```

### Create a Branch
```bash
git branch <branch_name>
```

### Switch Branch
```bash
git switch <branch_name>  # Recommended
git checkout <branch_name>
```

### Create and Switch to a Branch
```bash
git switch -c <branch_name>
git checkout -b <branch_name>
```

### Delete a Branch
```bash
git branch -d <branch_name>       # Delete local branch
git push origin --delete <branch_name>  # Delete remote branch
```

---

## **Remote Repositories**

### Add Remote
```bash
git remote add origin <repository_url>
```

### Fetch from Remote
```bash
git fetch origin
```

### Pull Changes
```bash
git pull origin <branch_name>
```

### Push Changes
```bash
git push origin <branch_name>
```

---

## **Merging and Rebasing**

### Merge Branch
```bash
git merge <branch_name>
```

### Rebase Branch
```bash
git rebase <branch_name>
```

---

## **Undoing Changes**

### Unstage Files
```bash
git reset <file>
```

### Discard Changes
```bash
git checkout -- <file>
```

### Undo Last Commit (Keep Changes)
```bash
git reset --soft HEAD~1
```

### Undo Last Commit (Discard Changes)
```bash
git reset --hard HEAD~1
```

---

## **Stashing**

### Save Changes Temporarily
```bash
git stash
```

### View Stashed Changes
```bash
git stash list
```

### Apply Stashed Changes
```bash
git stash apply
```

---

## **Tagging**

### Create a Tag
```bash
git tag <tag_name>
```

### Push Tags
```bash
git push origin <tag_name>
git push --tags  # Push all tags
```

---
