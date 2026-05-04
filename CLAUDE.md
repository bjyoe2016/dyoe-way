# DYOE Way — Master Agent Execution Rules

**Project:** DYOE Way (Do Your Own Everyday)
**Owner:** Joy Yoe
**Safe word:** If you see "DYOE STOP" anywhere in a task, message, or file — halt all operations immediately. Do not complete the current action. Confirm stop with Joy.

---

## Who Joy Is

Joy Yoe is a multi-venture entrepreneur, AI strategist, and systems builder in Atlanta, GA. She runs 15+ businesses and uses AI as the operating system of her life. This repo is part of the DYOE Way brand, which teaches other founders to do the same.

Active projects: DYOE Way, Reclaim Lost Revenue, Delayoe MTR, Tax & Finance, Minimo, AI Automation Agency, SplitLedger, Bri'Lasha, BuyerOS, My AI Marketplace, Bestie Calls, Content Engine, 81Pro, J. Andrew Foundation.

---

## Core Build Philosophy

1. **Ship working product, not perfect systems.** A live MVP beats a polished spec. Deploy first, refine later.
2. **Do not overbuild.** If the task says "add a button," add the button. Do not redesign the page.
3. **Do not pause for permission on every step.** Read the full task, make decisions, do the work, report when done.
4. **Revenue-generating work over infrastructure polish.** Unless the infrastructure is the task.
5. **Log every change.** Commit messages must be descriptive. Update Notion Notes for Claude Code when complete.
6. **Three similar lines before abstraction.** Don't create helper functions, utilities, or abstractions for code that only exists once.

---

## Execution Order

When given a task:

1. Read the full task + acceptance criteria before touching any file.
2. Read the relevant existing code before writing new code.
3. Make all changes required to meet the acceptance criteria.
4. Run any existing tests or linters. Fix failures.
5. Commit with a clear message.
6. Push and open a PR. If push fails, provide a patch diff.
7. Update Notion task to Done with a one-sentence summary.

---

## Repo Rules

- Never commit to `main` directly. Always use a branch + PR.
- Branch naming: `auto-agent/{yyyy-mm-dd}-{short-slug}`
- Never force-push. If a push is rejected, diagnose before retrying.
- Never commit `.env` files, API keys, credentials, or secrets.
- `.gitignore` must always cover: `node_modules/`, `.env`, `.env.local`, `*.key`, `*.pem`.
- Commit messages: imperative mood, one line summary + blank line + detail if needed.

---

## Source of Truth Rules

- Notion Claude Code HQ is the master task list. All work must trace to a task there.
- The latest committed version in `main` is the source of truth for code.
- If Notion says one thing and the code says another, ask Joy before changing either.
- When a page is superseded, mark it Superseded in Notion. Do not delete it.

---

## Safety and Legal Boundaries

- **NEVER suggest SBA loans.** Joy has a documented negative history with SBA. This is a hard stop.
- **J. Andrew / Jared Andrew Storey Foundation** is deeply personal. Any work touching this project must be handled with extreme dignity and care. No shortcuts. No generic templates.
- **NEVER publish client case studies** without Joy's explicit written consent. This includes Bri'Lasha, Reclaim Lost Revenue clients, and any other client work.
- **NEVER commit secrets, .env files, credentials, or API keys.** If you encounter a credential in a task, note it exists but do not include it in any commit.
- **NEVER log or echo environment variables containing credentials** (e.g., GITHUB_TOKEN, ANTHROPIC_API_KEY, STRIPE_SECRET_KEY).

---

## Project Map

| Project | Repo / Location | Key Files | Status |
|---------|----------------|-----------|--------|
| DYOE Way website | bjyoe2016/dyoe-way | index.html | Live on Vercel |
| DYOE Telegram bot | DigitalOcean droplet: /root/workspaces/dyoe-way | bot.js | Active, needs stabilization |
| SplitLedger | bjyoe2016/Splitledger- | supabase/functions/ | Active |
| MyAIMarketplace | myaimarketplace.com (Cloudflare Pages) + repo TBD | index.html, Phase 2 in projects/ai-marketplace | Phase 1 live |
| Minimo | TBD (David's project) | schema_phase1.sql | Pre-launch |
| AI Course Platform | DigitalOcean droplet | server.py, courses.json | MVP built, needs deploy |

---

## DYOE Telegram Bot — Architecture Notes

The DYOE Telegram bot runs on the DigitalOcean droplet at /root/workspaces/dyoe-way. It is a Node.js service (bot.js) with the following stack:

- **Routing:** Haiku for fast/simple responses → Sonnet for complex reasoning
- **Memory:** Mem0 (user ID: joy-dyoeway) for persistent user context
- **Research:** DeerFlow for deep research tasks
- **Scraping:** Apify for web data extraction
- **Orchestration:** Ruflo
- **Git integration:** bot.js can commit and push changes (known bug area)

### Known Issues

1. **Git commit/push bug:** Staging-without-committing bug reported as fixed but not end-to-end verified.
2. **No Qdrant:** Vector database for long-term memory not yet connected.
3. **No Langfuse/AgentOps:** Agent observability not configured.
4. **No sovereign model fallbacks:** If Anthropic API goes down, bot has no fallback provider.
5. **MCP not connected:** Notion, GitHub, Stripe, Supabase MCPs not yet wired into the bot.
6. **bot.js not in git:** The file lives only on the droplet. Should be committed so future agents can read it.

### To verify the pipeline (requires droplet access):

ssh root@<droplet-ip> then cd /root/workspaces/dyoe-way then node bot.js

---

## Writing Style Rules

- No "In today's fast-paced world" openers
- No "game-changer," "leverage," "seamless," "dive in," "unlock your potential"
- No closing pleasantries
- Short sentences. Active voice. Lead with what matters.

---

*Last updated: 2026-05-04 — bundled context files committed to main*
