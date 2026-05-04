# KILLSWITCH — DYOE Way Agent Stack Emergency Stop

**Safe word: DYOE STOP**

If Joy types or writes "DYOE STOP" anywhere — in a Notion task, a Telegram message, a GitHub issue, a comment, or any communication — every active agent must stop immediately. No exceptions.

---

## What "DYOE STOP" Triggers

1. **All Claude Code sessions:** Halt the current task. Do not commit. Do not push. Do not update Notion. Confirm stop.
2. **Telegram bot:** Stop processing the current message. Send: "DYOE STOP received. All operations halted."
3. **Daily autonomous task agent:** Do not pick up a new task. Leave status as-is and report current state.
4. **Any running automation:** If triggered by DYOE STOP, do not execute the next step.

---

## Layer-by-Layer Shutdown Procedures

### Layer 1 — Claude.ai Web Sessions
Close the browser tab. Do not save partial work as an Artifact.

### Layer 2 — Claude Code CLI
Ctrl+C. Do not commit staged changes until Joy confirms restart.

### Layer 3 — Autonomous Task Agent
Agent self-halts on DYOE STOP detection. Joy manually resets Status in Notion.

### Layer 4 — Telegram Bot (DigitalOcean droplet)
ssh root@<droplet-ip> → pm2 stop bot  (or pkill -f "node bot.js")
Restart: pm2 start bot

### Layer 5 — DeerFlow Research Agent
Stop active jobs via DeerFlow dashboard.

### Layer 6 — Apify Scraping
Stop running actors from Apify console.

### Layer 7 — Mem0 Memory
No action required. Memory persists safely.
To wipe: DELETE /memory?user_id=joy-dyoeway via Mem0 API.

### Layer 8 — Ruflo Orchestration
Halt active orchestration flows.

### Layers 9–18 (MCP Servers, Stripe, Supabase, GitHub, Notion)
Read/write tools only — no autonomous action. No new tool calls after STOP.

---

## After a STOP — Restart Checklist

- [ ] Reason for stop is resolved
- [ ] In-progress Notion tasks reviewed and reset
- [ ] No uncommitted changes stranded in any repo
- [ ] Telegram bot restart confirmed
- [ ] All agents briefed on pre-stop state

---

## Emergency Contacts

- **Joy Yoe** — Primary. All stops are Joy's call.
- **Barrett** — Can trigger STOP for 81Pro operations.
- **David** — Can trigger STOP for Minimo operations.

---

## Important: This File Is Read-Only for Agents

No agent may modify or delete this file without Joy's explicit written instruction.
If this file is missing from a repo, create it immediately before any other work.

---

*Last updated: 2026-05-04 — bundled context files committed to main*
