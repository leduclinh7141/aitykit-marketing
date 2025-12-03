---
description: Create a pull request
argument-hint: [branch] [from-branch]
---

## Variables

TO_BRANCH: $1 (defaults to `main`)
FROM_BRANCH: $2 (defaults to current branch)

## Workflow

1. Run `git status` to check current state
2. Run `git log` to see commits to include
3. Run `git diff {TO_BRANCH}...HEAD` to review changes
4. Push current branch if needed: `git push -u origin {FROM_BRANCH}`
5. Create PR using GitHub CLI: `gh pr create --title "..." --body "..."`

## Notes
- If `gh` command is not available, instruct the user to install and authorize GitHub CLI first.
