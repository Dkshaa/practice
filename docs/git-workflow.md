# Everyday Git Workflow

## Start from the latest code

```bash
git switch main
git pull --ff-only
git switch -c feature/short-description
```

## Review and save a change

```bash
git status
git diff
git add <file>
git commit -m "Describe the change"
```

## Share the branch

```bash
git push -u origin feature/short-description
```

Before opening a pull request, review the changed files and run the project's tests.

## Check what will be published

Compare the branch with `main` before opening the pull request:

```bash
git log --oneline main..HEAD
git diff --stat main...HEAD
git status
```

This confirms which commits and files belong to the branch and catches uncommitted
work before review.
