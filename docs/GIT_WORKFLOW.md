# Git Workflow - TASK 4

## Flow

Developer
   |
   v
feature/*
   |
   | Pull Request
   v
dev
   |
   | QA / review / approval
   | Pull Request
   v
main
   |
   | release tag
   v
v1.0.0

## What happens in each branch?

### main
Production-ready code only. Do not directly develop features here.

### dev
Integration branch. Features are combined and tested here before release.

### feature/*
Short-lived branch for one change, such as `feature/login` or `feature/navbar`.

## Typical real-world sequence

1. Clone the repository.
2. Switch to `dev`.
3. Create a feature branch.
4. Develop the change.
5. Commit with a meaningful message.
6. Push the feature branch.
7. Open a Pull Request into `dev`.
8. Review and test the change.
9. Merge the Pull Request.
10. Test the integrated `dev` branch.
11. Open a Pull Request from `dev` to `main`.
12. Merge after approval.
13. Create a version tag such as `v1.0.0`.
