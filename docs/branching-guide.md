# Git Branching Guide

Branches let you develop a change without disturbing the stable branch.

## Create a branch

```bash
git switch main
git pull --ff-only
git switch -c feature/add-login-form
```

Use a short prefix that describes the work:

- `feature/` for new functionality
- `fix/` for bug fixes
- `docs/` for documentation
- `refactor/` for internal improvements

## Keep the branch current

```bash
git fetch origin
git rebase origin/main
```

After the work is merged, remove the local branch with `git branch -d branch-name`.

To remove the corresponding remote branch after merging, run:

```bash
git push origin --delete branch-name
```

Use `-d` for local cleanup because Git refuses to delete an unmerged branch. Avoid
the force-delete option unless you have confirmed the branch contains no work you
still need.
