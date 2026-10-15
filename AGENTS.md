# Coding together

- Josh and Ned may be working in this repository at the same time. Read the relevant files and check Git status before editing.
- Keep changes focused on the assigned task. Preserve unrelated and in-progress work from other people or agents.
- When multiple agents are active, work on different files. Coordinate before editing shared configuration or dependency files.
- No app framework has been chosen yet. Don't scaffold an application or add dependencies unless the task calls for it.
- Never put credentials or real secrets in tracked files. Use ignored `.env` files and placeholder-only `.env.example` files.
- Run the checks relevant to your changes, and report what passed or couldn't be run.
- After completing a task and running the relevant checks, commit and push the task's changes to the current branch's GitHub remote by default, unless the user asks to keep the work local. No additional confirmation is needed. Stage only the task's files; preserve unrelated and in-progress work.
- Don't force-push, switch branches, or perform destructive Git operations unless explicitly asked. If publishing is blocked by conflicts, branch protections, or authentication, report the blocker instead of overwriting work.
