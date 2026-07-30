# Pull Request Guide

A pull request presents a branch for review before it is merged.

## Before opening a pull request

1. Pull or rebase onto the latest target branch.
2. Run the relevant tests and formatting checks.
3. Review the complete diff.
4. Remove debugging code and unrelated files.

## Write a useful description

Include:

- What changed
- Why the change was needed
- How the change was tested
- Screenshots for visible interface changes

## During review

Respond to questions clearly, make requested updates in focused commits, and confirm that automated checks pass before merging.

## Before merging

- Re-read the final diff, including changes added during review.
- Confirm every review conversation is resolved.
- Check that the branch can merge without conflicts.
- Choose a merge strategy that matches the repository's conventions.
- Delete the source branch after the change is safely merged.
