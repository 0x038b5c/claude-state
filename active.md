## What I was doing
Maintaining claude-payload (context.md / prompt engineering)

## What's done
- Added <git_commits> section to context.md with Conventional Commits prompt (lowercase subjects, 50-char limit, imperative mood, optional body)

## What's in flight
- N/A

## What's next
- Remaining open suggestions for claude-loader/claude-payload:
  - sops is installed but unused — remove or document intent
  - git user.email is claude@anthropic.com — consider a throwaway address
  - payload main.py doesn't auto-load project CLAUDE.md / todo.md at startup when a project is active
  - tool has no state management commands (e.g. `tool state set-project`, `tool state clear`)
