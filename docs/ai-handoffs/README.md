# AI Handoff Records

`AI_HANDOFF.md` is the short, current snapshot. This directory contains
append-only records for individual tasks so Codex and Claude Code can hand work
over without rereading the whole repository.

Create one file per task from `TEMPLATE.md`, named
`YYYY-MM-DD-short-task-name.md`. Keep records concise and reference files and
commit SHA values instead of pasting source code or command output.

Do not record credentials, access tokens, personal media, local paths that only
work on one machine, or uncommitted secrets. A record cannot preserve running
processes, browser sessions, environment variables, or remote provider jobs;
write down how the next agent can safely inspect or recreate them instead.
