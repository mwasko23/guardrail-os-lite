# Guardrail OS — Lite

**A discipline layer for AI coding agents. Free core, MIT-licensed.**

*Ship fast without shipping broken.*

Created by Marta Waśko · [HitIt.ai](https://hitit.ai)

---

If you've watched an AI coding agent move fast and break things — merging on green tests that never exercised the real path, "fixing" a bug with a workaround, refactoring five files when you asked for one, or just silently stalling mid-task — the problem isn't the model. It's that the agent has no operating discipline.

**Guardrail OS Lite is that discipline, in one file.** Drop `GUARDRAIL_LITE.md` into your agent's instructions (`CLAUDE.md`, a system prompt, a rules file — anything it reads) and it will plan before it codes, run real quality gates, respect size limits, apply a security checklist to every mutation, and stop-and-ask instead of guessing.

## What's in Lite (free)

- **The priority order** — security > accuracy > simplicity > maintainability > performance > ship date. The single most useful rule you can give an agent.
- **Quality gates** — the checks that must pass every commit.
- **Size limits** — small files, small commits, small PRs.
- **The mutation security checklist** — auth, anti-forgery, rate limit, validation, owner-scoping, audit log.
- **Plan → approval → code** — no code before a signed-off plan.

One file. Works with Claude Code, Cursor, Codex, Gemini CLI — anything that reads markdown instructions.

## Quickstart

1. Copy `GUARDRAIL_LITE.md` into your project.
2. Reference it from your agent's instruction file (e.g. add "Follow GUARDRAIL_LITE.md" to your `CLAUDE.md`).
3. Start a task. The agent now plans, gates, and escalates instead of winging it.

## Lite vs. the full kit

Lite gives one agent a spine. The **full Guardrail OS kit** turns that into a *team* — three roles that coordinate through shared files in your repo, so it runs in any tool:

| | Lite (free) | Full kit |
|---|---|---|
| Core ruleset (priority order, gates, limits, security) | ✅ | ✅ |
| Single-agent discipline | ✅ | ✅ |
| **Three roles** — PM / Supervisor / Coder with a real authority split | — | ✅ |
| **File-based coordination hub** — `_hub/` message bus (LOG · BOARD · DECISIONS · FINDINGS) that survives context resets | — | ✅ |
| **Paste-to-start bootstrap prompts** — spin up each role in any tool (Claude Code, Cursor, Codex, Gemini CLI, Cowork), no slash commands | — | ✅ |
| **Escalation protocol** + report-back cadence (no more silent stalls) | — | ✅ |
| **Self-evolving governance** — codify a rule the first time something breaks | — | ✅ |
| **Stack config + reference adapter** (Next.js/Supabase worked example) | — | ✅ |
| **5 templates** — task, PR review, escalation, incident, ADR | — | ✅ |
| **Case studies** — three real rules, how each was born from a real failure | — | ✅ |
| **10-minute setup guide** | — | ✅ |
| Lifetime updates | — | ✅ |

**→ Get the full kit:** https://hititai.gumroad.com/l/ghizpe

## License

Lite is MIT licensed — use it, fork it, ship it. See `LICENSE`. The full kit is sold under separate commercial terms.

---

*Built the hard way: this system grew out of running a real three-agent team that shipped a production app. The rules are earned, not invented. If Lite helps, the full kit is the whole team.*
