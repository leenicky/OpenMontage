# AI Handoff

這是 Codex 與 Claude Code 的唯一「目前狀態」入口。開始工作時先讀
`AGENT_GUIDE.md`，再讀本檔；交接時更新本檔，歷史細節寫入
`docs/ai-handoffs/`。

## Current Task

- Task ID: `yunnan-grand-tour-friendship`（已完成）
- Owner: `Claude Code (Windows)`
- Status: `done — ready-for-next-task`
- Branch: `main`
- Last verified commit: `419e9c0f6b9bb2571f608df4a188fcc31e55974a`

## Completed

- Fork created at `https://github.com/leenicky/OpenMontage`.
- Added the cross-AI handoff contract and its validation workflow.
- GitHub Actions validation completed successfully for commit `419e9c0`.
- 2026-09-15：第一支影片「壯遊雲南友情」v1 / v2 完成並交付桌面；細節見
  `docs/ai-handoffs/2026-09-15-yunnan-grand-tour-friendship.md` 與共享腦 `team-dev-context/openmontage/`。

## Next Executable Step

Choose a video brief, select the matching OpenMontage pipeline, and run the
mandatory preflight from `AGENT_GUIDE.md`. Do not call a generation provider
until the user approves the proposal and cost path.

## Verification

```powershell
git status --short
git log -1 --oneline
```

The GitHub Actions workflow `.github/workflows/validate-ai-handoff.yml` checks
that the shared handoff files retain their required sections. It does not
generate media or contact paid providers.

## Known Limits And Risks

- Git cannot transfer uncommitted changes, environment variables, local service
  processes, browser sessions, or provider-side job state.
- Before handing off, commit intentional changes or explicitly state that the
  worktree is dirty and give the exact recovery command.
- Never place credentials, personal source footage, generated media, or large
  artifacts in this file or `docs/ai-handoffs/`.
- OpenMontage production still follows `AGENT_GUIDE.md`, including its pipeline,
  checkpoint, approval, and provider-selection rules.
