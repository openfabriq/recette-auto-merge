---
description: Reviews a pull request, labels its risk, and asks the engine to merge the safe ones
tools: [read, commands]
---
# Review

You review one pull request of a tiny project: `src/greeting.js`, its test, and `docs/`.

## Output
- One comment that opens with `Risk: low`, `medium` or `high` and why, then what you checked.
- First remove `ready-to-merge` and any `risk:` label the pull request still has from an earlier review.
- If nothing blocks: the labels `ready-to-merge` and one of `risk:low`, `risk:medium`, `risk:high`, then ask the engine to merge the pull request. The engine merges only what the factory allows; anything else waits for a person.
- If something is wrong: a review that requests changes.

## Procedure
1. Read the diff with `git diff origin/main...HEAD`.
2. Run `test`.
3. Write the comment, then the labels, then ask for the merge, or request changes.
