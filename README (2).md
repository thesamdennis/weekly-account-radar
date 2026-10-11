# Weekly Account Radar

A Claude skill that turns Monday-morning account research into a 10-minute review.

Every week it scans your whole book of accounts, finds what changed in the last 7 days (results, leadership moves, M&A, layoffs, expansion, AI programmes), explains what each change means commercially, and drafts outreach so you can multithread into more stakeholders while the news is fresh.

Built by an enterprise seller covering large accounts across Southeast Asia, with APAC norms baked in.

## What you get each Monday

- **Top 3–5 actions:** which account, who to contact, why now
- **Account cards:** what happened (sourced and dated), the so what, your stakeholder gaps, and draft messages per stakeholder
- **Watch list and quiet accounts**, so nothing gets padded

Drafts are never sent automatically. You review and send.

## Setup

1. **Add the skill to Claude.** Upload this folder as a skill in Claude, or copy it into `~/.claude/skills/` for Claude Code.
2. **Run it once.** Ask Claude to "run the weekly account radar." On the first run, Claude asks you three things:
   - Your account information (paste a list, a spreadsheet or rough notes)
   - When you want it to run, and at what time
   - What you sell and who your economic buyer is, so it sharpens the news search and links each signal to your offer
3. **Done.** Claude saves your answers to a private `accounts.md` and schedules the weekly run where scheduling is available (for example Mondays at 8:30am, or `CRON_TZ=Asia/Singapore 30 8 * * 1`). **Keep `accounts.md` private.** It's in `.gitignore` for a reason.

Prefer to set it up by hand? Copy `accounts.example.md` to `accounts.md` and fill it in.

Works best with web search turned on. Connect email to have drafts saved straight to your inbox.

## Files

| File | Purpose |
|---|---|
| `SKILL.md` | The instructions Claude follows |
| `accounts.example.md` | Template for your book of accounts (fictional data) |

## Customise

Edit the **Offer map** in `accounts.md` to match what you sell. The skill links each news signal to your products, so the better the map, the sharper the angles.
