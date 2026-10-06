# Interview Questions - Git

## 1. What is Git?
Git is a distributed version control system used to track code changes and collaborate safely.

## 2. Merge vs Rebase
Merge combines histories and normally creates a merge commit. Rebase moves commits onto a new base and creates a linear history. In team workflows, avoid rebasing shared branches unless the team agrees.

## 3. What is a Pull Request?
A Pull Request is a request to merge changes from one branch into another. It provides a place for review, discussion, checks, and approval.

## 4. How do you resolve merge conflicts?
1. Run `git status`.
2. Open the conflicted file.
3. Decide which changes should remain.
4. Remove conflict markers.
5. Run `git add`.
6. Commit the resolved result.
7. Push the branch and continue the PR.

## 5. What are Git tags?
Tags are named references to specific commits. They are commonly used for releases such as `v1.0.0`.

## 6. Explain Git workflow.
A common workflow is feature branch -> Pull Request -> dev -> testing/review -> Pull Request -> main -> release tag.

## 7. Explain git stash.
`git stash` temporarily stores uncommitted changes so you can switch branches without committing unfinished work.

## 8. What is .gitignore?
`.gitignore` lists files and directories Git should not track, such as virtual environments, build output, IDE settings, logs, and secrets.
