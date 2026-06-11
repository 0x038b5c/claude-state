## What I was doing
Reviewing and improving the claude-loader and claude-payload repos

## What's done
- Reviewed both repos and identified improvement areas
- Confirmed keys/ was never committed to git (already in .gitignore) — no rebase needed
- Added `chmod 600` on signing key after rage decrypt (main.py)
- Replaced bundled binaries (gh, rage, sops) with apt installs; kept bin/tool and restored its copy to /usr/local/bin
- Scaffolded full project structure in `tool project new`: CLAUDE.md, .claude/todo.md, .claude/notes/, initial signed commit+push, state.json+active.md update
- Dropped `updated_at` from state.json schema (nothing consumed it)
- Broke up chained `&&` shell commands into separate `run()` calls

## What's in flight
- N/A

## What's next
- Remaining suggestions not yet acted on:
  - sops is installed but unused — remove or document intent
  - git user.email is claude@anthropic.com — consider a throwaway address
  - payload main.py doesn't auto-load project CLAUDE.md / todo.md at startup when a project is active
  - tool has no state management commands (e.g. `tool state set-project`, `tool state clear`)
