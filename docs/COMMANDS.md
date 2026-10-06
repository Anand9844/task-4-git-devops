# Git Commands Used

## Configure Git
```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

## First push
```bash
git init
git add .
git commit -m "chore: initial project setup"
git branch -M main
git remote add origin https://github.com/<YOUR-USERNAME>/task-4-git-devops.git
git push -u origin main
```

## Create dev
```bash
git checkout -b dev
git push -u origin dev
```

## Create a feature branch
```bash
git checkout dev
git pull origin dev
git checkout -b feature/login
```

## Commit and push feature
```bash
git add .
git commit -m "feat: add login page"
git push -u origin feature/login
```

## View branches
```bash
git branch
git branch -a
```

## View history
```bash
git log --oneline --graph --decorate --all
```

## Merge locally (if needed)
```bash
git checkout dev
git pull origin dev
git merge feature/login
git push origin dev
```

For the assignment, prefer Pull Requests on GitHub to demonstrate the review workflow.

## Tag
```bash
git checkout main
git pull origin main
git tag -a v1.0.0 -m "Production release v1.0.0"
git push origin v1.0.0
```

## Stash
```bash
git stash
git stash pop
```

## Conflict resolution
```bash
git status
# edit conflicted files
git add .
git commit -m "fix: resolve merge conflict"
```
