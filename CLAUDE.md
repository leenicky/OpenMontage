# OpenMontage

**MANDATORY: Read [`AGENT_GUIDE.md`](AGENT_GUIDE.md) before responding to ANY user message.**

Do not act on the user's request until you have read AGENT_GUIDE.md.
It contains routing rules that determine your first action based on what the user asked.
Skipping it WILL cause you to take the wrong action.

There are no instructions in this file. All instructions are in AGENT_GUIDE.md.

## 跨 AI 交接

在讀完 `AGENT_GUIDE.md` 後，先讀取 [`AI_HANDOFF.md`](AI_HANDOFF.md)。它是
Codex 與 Claude Code 共用的目前任務快照；依其中的檔案路徑、commit SHA 與驗證
命令按需讀取，不要為了接手而掃描整個版本庫。

交接前必須更新 `AI_HANDOFF.md`，並在 `docs/ai-handoffs/` 建立或補充該任務的
append-only 紀錄。不可在這些檔案記錄 API key、token、原始媒體、使用者私密資料、
未提交變更或執行中程序；這些狀態無法可靠跨 session 傳遞，必須明確標為待重新建立。
