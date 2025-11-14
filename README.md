# Agentic DevOps Demo: Hello World-3

This repo demonstrates a minimal "agentic" DevOps workflow using GitHub Actions as an agent. 
Whenever a PR is opened or updated, if any commit message contains `hello`, the agent posts a welcome comment.

## How to Use

1. Fork this repo (or use directly).
2. Make a Pull Request (PR) with a commit message that includes `hello` (e.g., "add: hello world feature").
3. Go to the PR page – you’ll see a comment:  
   `👋 Hello, welcome! This is an Agentic DevOps demo.`

## What’s Happening?

- The GitHub Actions workflow runs on every PR.
- The “agent” step (using `github-script`) inspects the commit messages.
- If any commit message contains `hello` (case-insensitive), it posts a comment on the PR.

## Files

| File                                  | Purpose                                  |
|----------------------------------------|------------------------------------------|
| `main.py`                             | Simple Hello World Python script.        |
| `.github/workflows/agentic-demo.yml`   | The agentic workflow.                    |
| `README.md`                           | This file.                               |

## Extend the Demo

- Try changing the keyword or comment.
- Expand the script to run tests, trigger webhooks, or gate merges.
- Use this pattern to introduce students to more advanced agentic automation!

---
