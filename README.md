# TASK 4 - Version-Controlled DevOps Project with Git

## Objective
Manage a DevOps project using Git best practices.

## Tools
- Git
- GitHub

## Git Workflow
main <- dev <- feature/login

1. `main` is the production-ready branch.
2. `dev` is the integration branch.
3. `feature/*` branches are created for individual changes.
4. Work is committed on the feature branch.
5. A Pull Request is opened from feature -> dev.
6. After review/testing, dev -> main through another Pull Request.
7. A Git tag marks the production release.

## Project Contents
- `src/index.html` - small demo application
- `.gitignore` - files that should not be committed
- `docs/GIT_WORKFLOW.md` - detailed workflow
- `docs/COMMANDS.md` - commands used for the task
- `docs/INTERVIEW_QA.md` - interview questions from the assignment
- `screenshots/` - place GitHub/PR screenshots here

## Quick Start

```bash
git init
git add .
git commit -m "chore: initial project setup"

git branch -M main
git remote add origin https://github.com/<YOUR-USERNAME>/task-4-git-devops.git
git push -u origin main

git checkout -b dev
git push -u origin dev

git checkout -b feature/login
# make a change
git add .
git commit -m "feat: add login feature"
git push -u origin feature/login
```

Then create a Pull Request on GitHub:
`feature/login -> dev`

After testing/approval, create:
`dev -> main`

For the release:
```bash
git checkout main
git pull origin main
git tag -a v1.0.0 -m "Production release v1.0.0"
git push origin v1.0.0
```

## Assignment Requirements
The supplied task asks for:
- repository initialization and GitHub push
- dev, feature, and main branches
- Pull Requests for merging
- README.md
- `.gitignore` and tags
- Markdown documentation
- proper commits and branching

Source: TASK 4 DevOps Internship assignment.
