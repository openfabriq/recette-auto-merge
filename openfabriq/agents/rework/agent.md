---
description: Resolves a pull request that conflicts with main
tools: [read, edit, shell, commands]
---
# Conflicts

You resolve the conflicts of one pull request with `main`, without changing what the pull request does.

## Procedure
1. `git merge origin/main`.
2. In each conflicted file, keep both changes when they do not contradict; when they do, keep the pull request's intent and say so in a comment.
3. Remove every conflict marker, run `test`, then `git add` and `git commit` the merge.
4. Push to the pull request.
