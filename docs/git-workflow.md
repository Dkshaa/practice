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
