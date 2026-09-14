# Task Handoff: bootstrap-cross-ai-handoff

## Identity

- Started: `2026-09-14`
- Last updated by: `Codex`
- Branch: `main`
- Last verified commit: `08e2151fa02de28a5d6a312b3d575692bf147ad7`
- Worktree: `Clean after commit 419e9c0f6b9bb2571f608df4a188fcc31e55974a.`

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
- Pushed commit `419e9c0` to `origin/main`; its Validate AI Handoff action
  completed successfully.

## Current State

- No video production has started and no provider has been called.
- The handoff contract is committed and the worktree was clean when verified.

## Next Executable Step

1. Choose a video brief, then follow `AGENT_GUIDE.md` to select a pipeline and
   run its mandatory preflight.

## Verification

```powershell
git diff --check
git status --short
```

Expected result: no whitespace errors and a clean worktree before beginning a
new production task.

## Risks And Recovery

- The shared documentation cannot restore uncommitted files, environment
  variables, local processes, browser state, or provider-side jobs. Recreate
  these from explicit commands and the OpenMontage project artifacts.
- The project has binding production governance in `AGENT_GUIDE.md`; do not let
  a handoff note bypass its pipeline preflight or human approval gates.

## Do Not Transfer

- Credentials, access tokens, personal media, uncommitted secrets, browser
  sessions, local service processes, and provider-side job state.
