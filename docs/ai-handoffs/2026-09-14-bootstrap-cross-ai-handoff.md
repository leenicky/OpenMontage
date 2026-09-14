# Task Handoff: bootstrap-cross-ai-handoff

## Identity

- Started: `2026-09-14`
- Last updated by: `Codex`
- Branch: `main`
- Last verified commit: `08e2151fa02de28a5d6a312b3d575692bf147ad7`
- Worktree: `Pending commit for the handoff contract files listed below.`

## Objective

Make this fork usable by both Codex and Claude Code when either session ends or
runs short of context.

## Completed

- Created fork `leenicky/OpenMontage` with upstream remote
  `calesthio/OpenMontage`.
- Added `AI_HANDOFF.md` as the rolling cross-AI task snapshot.
- Updated `AGENTS.md` and `CLAUDE.md` to read the existing OpenMontage guide
  before the shared snapshot.
- Added this handoff record, its template, and a GitHub Actions contract check.

## Current State

- No video production has started and no provider has been called.
- The next agent must inspect `git status --short`, commit the pending handoff
  contract, then update `AI_HANDOFF.md` before starting a new task.

## Next Executable Step

1. Run `git diff --check`, review the pending files, commit them, and push the
   `main` branch to `origin`.

## Verification

```powershell
git diff --check
git status --short
```

Expected result: no whitespace errors; only the shared handoff files are
pending.

## Risks And Recovery

- The shared documentation cannot restore uncommitted files, environment
  variables, local processes, browser state, or provider-side jobs. Recreate
  these from explicit commands and the OpenMontage project artifacts.
- The project has binding production governance in `AGENT_GUIDE.md`; do not let
  a handoff note bypass its pipeline preflight or human approval gates.

## Do Not Transfer

- Credentials, access tokens, personal media, uncommitted secrets, browser
  sessions, local service processes, and provider-side job state.
