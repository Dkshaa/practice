# Commit Message Guide

A good commit message explains the outcome of a focused change.

## Recommended format

```text
Short action-oriented summary

Optional details explaining why the change was needed.
```

## Examples

- `Add validation to the signup form`
- `Fix cart total rounding`
- `Document local development setup`
- `Remove unused navigation styles`

## Tips

- Start with a verb such as Add, Fix, Update, or Remove.
- Keep the first line concise.
- Describe what changed, not the editing process.
- Avoid mixing unrelated changes in one commit.

## Add context when needed

Use the optional body to explain the reason for a change, important tradeoffs, or
behavior that is not obvious from the diff. Leave a blank line between the summary
and body so Git tools display the message correctly.

```text
Prevent duplicate task submissions

Disable the submit button while the request is in progress so repeated clicks do
not create duplicate tasks.
```
