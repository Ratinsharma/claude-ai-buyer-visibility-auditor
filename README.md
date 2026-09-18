# AI Buyer Visibility Auditor

Claude skill that scores AI buyer visibility /10 and emits a truthful `llms.txt`.

Free audit tool for Claude Code / Claude.ai. Runs a 10-query framework across Category, Problem, Trust, and Compliance layers, explains failures, and generates publishable `llms.txt` with zero fabricated claims.

## Features

- 10-query audit across 4 layers (Category / Problem / Trust / Compliance)
- Score out of 10 with per-query failure reasons
- Two-speed onboarding: company name + URL first, then verify researched facts
- Generates production-ready `llms.txt` from verified proof only
- Flags gaps instead of inventing claims

## Stack

- Claude Code skill (`SKILL.md`)
- No app runtime — install as a skill, trigger in chat

## Quickstart

### Option 1: Claude Code (recommended)

```bash
npx skills add Ratinsharma/claude-ai-buyer-visibility-auditor
```

Restart Claude Code if needed, then say: **Audit our AI visibility**

### Option 2: Manual clone

```bash
git clone https://github.com/Ratinsharma/claude-ai-buyer-visibility-auditor.git
mv claude-ai-buyer-visibility-auditor ~/.claude/skills/
```

### Option 3: Claude.ai (web)

Copy `SKILL.md` into a Project's custom instructions (or paste as system prompt), then trigger with **Audit our AI visibility**.

## Structure

```
claude-ai-buyer-visibility-auditor/
├── SKILL.md      # Skill definition Claude reads
├── README.md     # This file
└── LICENSE       # MIT
```

## License

MIT — see [LICENSE](./LICENSE).

## Author

Ratin Sharma