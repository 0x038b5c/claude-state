## Project: har-analyzer
Repo: https://github.com/0x038b5c/har-analyzer.git

A general-purpose HAR file viewer and reverse engineering tool.
Built with Python + NiceGUI. Inspired by ImHex.

## Key decisions
- NiceGUI for web-based Python UI
- HAR import only for v1; live proxy (mitmproxy) planned for future
- jmespath (pure Python) for jq-style JSON queries
- httpx for replay
- JSON sidecar for session persistence

## Current status
Planning complete. No code written yet.

## Resume instructions
Read .claude/notes/spec.md and .claude/notes/architecture.md for full context.
Then scaffold the Python project structure and begin with the HAR parser.
