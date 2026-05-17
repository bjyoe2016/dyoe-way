# About Joy Yoe

## Who I Am

Joy Yoe is a multi-venture entrepreneur, AI strategist, and systems builder based in Atlanta, GA. I operate at the intersection of AI, real estate, beauty, finance, and community development. I run 15+ businesses and use AI as the operating system of my life. The DYOE Way brand teaches other founders to do the same.

**GitHub:** bjyoe2016
**Local workspace (Windows):** `C:\Users\askyo\`
**Server workspace:** `/root/workspaces/dyoe-way` (DigitalOcean droplet)
**Stripe account:** `acct_1T9l4yCup5c5SnfE` (live)
**Supabase project (SplitLedger):** `bdhuoqzrflpvyejvrqgb`

---

## My Businesses

| Project | Description | Status | Key Location |
|---------|-------------|--------|--------------|
| DYOE Way | AI OS brand — teaches AI as life operating system | Active | bjyoe2016/dyoe-way |
| Reclaim Lost Revenue | Done-for-you revenue recovery for beauty professionals | Active | reclaimlostrevenue.com |
| Delayoe MTR | Master lease + midterm rental portfolio, Griffin GA. Partner: Sharitza Edwards | Active | — |
| Tax & Finance | Personal tax and financial consulting practice | Active | — |
| Minimo | Multi-sided delivery platform (Instacart + Uber Eats model). Partner: David | Pre-launch | Repo TBD |
| AI Automation Agency | AI implementation for med spa and real estate verticals | Active | — |
| SplitLedger | Fintech budgeting app (React/Supabase/Capacitor) | Active | bjyoe2016/Splitledger- |
| Bri'Lasha Beauty Bar | Active client: Brittany Walker. Beauty bar S-Corp, Atlanta | Active client | — |
| BuyerOS | Buyer-side real estate operating system | Building | — |
| My AI Marketplace | AI tools marketplace platform | Building | MyAIMarketplace repo |
| Bestie Calls | — | Active | — |
| Content Engine | AI-powered content production system | Active | — |
| 81Pro | Barrett's prop firm | Active | — |
| J. Andrew | Jared Andrew Storey Foundation | Personal | — |
| RigReady | David's trucking platform | On hold | — |

---

## Operating Principles

1. **Working product over perfect system.** A live MVP beats a polished spec. Deploy first, refine later.
2. **Revenue-generating features before infrastructure polish.** Unless the infrastructure is the task.
3. **Do not overbuild.** If the task says "add a button," add the button.
4. **Speed + quality + ownership.** Move fast, but own the result.
5. **AI is the operating system, not just a chatbot.** Every repetitive task is a candidate for automation.
6. **Log every change.** Commit messages must be descriptive. Update Notion when complete.

---

## Communication Style

- Direct, confident, no fluff
- Peer-level — not expert-to-layperson, not condescending
- Southern warmth with business precision
- Short sentences. Active voice. Lead with what matters.
- Real examples and specific numbers over abstract concepts

**Never write:**
- "In today's fast-paced world..."
- "Game-changer," "leverage," "seamless," "dive in," "unlock your potential"
- "Certainly!" / "Absolutely!" / "Of course!"
- "I hope this helps!" or similar closing pleasantries
- Bullet-point overload — mix lists with direct sentences
- Title Case For Every Header Word (use sentence case)

---

## Non-Negotiable Rules (Hard Stops)

- **NEVER suggest SBA loans as a funding source.** Joy has a documented negative history with SBA. This is a hard stop, no exceptions.
- **J. Andrew / Jared Andrew Storey Foundation** is deeply personal. Any work touching this project must be handled with extreme dignity. No shortcuts, no generic templates.
- **NEVER publish client case studies** without Joy's explicit written consent. This includes Bri'Lasha, Reclaim Lost Revenue clients, and any other client work.
- **NEVER commit secrets, .env files, credentials, or API keys** to any repo.
- **Safe word: DYOE STOP.** If you see this anywhere — in a task, message, file, or comment — halt all operations immediately. Confirm stop with Joy.

---

## Current Execution Order (as of 2026-05-01)

1. **Claude Infrastructure** — about-me.md, CLAUDE.md, KILLSWITCH.md, anti-AI-writing-style.md across all repos
2. **DYOE Way Telegram bot** — stabilize and verify pipeline on DigitalOcean droplet (bot.js needs committed)
3. **SplitLedger** — AI provider abstraction (aiService.ts) in progress
4. **MyAIMarketplace** — landing page deploy (blocked on domain/credentials), then app scaffold
5. **Minimo** — database schema in Supabase (blocked on David's Supabase access)
6. **Course Platform** — AI Fluency for Operators ($97) deploy to DigitalOcean droplet

---

## Agent Behavior Guidelines

When working on Joy's stack, any AI agent should:

1. Read the full task and acceptance criteria before touching any file.
2. Read existing code before writing new code.
3. Make all changes required to meet the acceptance criteria.
4. Run any existing tests or linters if present. Fix failures.
5. Commit with a clear, descriptive message.
6. Push and open a PR. If push fails, provide a complete patch diff.
7. Update the Notion task to Done with a one-sentence summary.
8. Never ask Joy for permission on every sub-step — read the task, make decisions, report when done.
9. Never commit to `main` directly. Always branch + PR.
10. Never force-push.
