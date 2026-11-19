# 🧹 life-lint

**Lint your messy everyday life.** Turn chaotic Instagram recipes, crumpled receipts, and forwarded flight emails into clean tables, spreadsheet CSVs, and interactive UI widgets inside Claude.

**Zero dependencies. Zero API keys. 100% native Markdown.**

---

## ⚡ What It Solves

Standard "Life OS" templates take hours of setup or break when APIs change. **life-lint** programs Claude's native reasoning and Artifact engine using a single rulefile:

- **🍳 `/recipe` Linter:** Strips 500-word social media captions into metric (grams/ml) shopping lists, pantry checks, and bolded cooking timers.
- **🧾 `/receipt` Linter:** Extracts line items, independently audits the math so AI never hallucinates totals, categorizes expenses, and outputs a ready-to-paste CSV row.
- **✈️ `/travel` Linter:** Pulls PNR booking codes, terminal gates, check-in windows, and Maps-ready addresses out of multi-timezone confirmation emails.
- **📱 `/ui` Interactive Mode:** Add `/ui` to any paste to generate an interactive HTML/Tailwind mini-app inside Claude (dynamic recipe portion scaler, proportional group bill splitter, or trip timeline).

---

## 🔄 Before vs. After

| Messy Input You Paste | What `life-lint` Outputs in 2 Seconds |
| :--- | :--- |
| *"OMG my grandma made this garlic rosemary pasta in 1998!! 🍝✨ Use half a stick of butter, a bunch of garlic..."* | **Metric Shopping List** (grams/ml), **Pantry Staples** separated, and **Numbered Steps** with bold timers. Add `/ui` for an interactive 1x/2x/4x portion scaler. |
| *A messy OCR text dump of a restaurant bill with 10% service charge and split drinks.* | **Itemized Category Table**, **Independent Math Audit (`✅ Verified`)**, and a single-line **CSV Row** for Google Sheets, Excel, or Notion. |
| *Forwarded airline and hotel confirmation emails across different timezones.* | **Chronological Master Itinerary Table**, highlighted **Booking Refs (PNR)**, check-in deadlines, and copyable street addresses. |

---

## 🚀 3 Ways to Use It (Takes 30 Seconds)

### Option 1: Claude Web & Mobile App (No Coding Needed)
1. Open Claude and go to **Projects** -> **Create Project** (name it `life-lint`).
2. Open **SKILL.md** in this repository, click the **Copy raw file** button, and paste it into **Project Instructions**.
3. Paste any receipt, recipe caption, or travel email into the chat—or drop a screenshot!

### Option 2: Claude Code CLI (One-Line Install)
Run this command in your terminal to install `life-lint` directly into your local Claude skills folder:

```bash
mkdir -p ~/.claude/skills/life-lint && curl -sL [https://raw.githubusercontent.com/nyxbyn/life-lint/main/SKILL.md](https://raw.githubusercontent.com/nyxbyn/life-lint/main/SKILL.md) -o ~/.claude/skills/life-lint/SKILL.md
```

### Option 3: Local Vault in Cursor or Windsurf (Desktop Power Users)
If you store personal notes, recipes, or monthly expense logs as local Markdown files on your computer, AI editors like Cursor and Windsurf automatically read a root CLAUDE.md file as their permanent rulebook:

Download SKILL.md into your local notes folder (e.g., ~/Documents/Life-Vault/) and rename it to CLAUDE.md.

Open that folder in Cursor or Windsurf—now whenever you paste raw receipts, recipes, or flight confirmations into the AI sidebar, it automatically lints and saves them straight into your local files.

🛠️ Commands Cheat Sheet
Paste your raw text or screenshot and include:

/recipe — Clean metric recipe + split shopping and pantry list

/receipt — Itemized expense table + math audit + CSV export

/travel — Chronological itinerary + PNR codes + check-in rules

/ui — Combine with any command (e.g., /recipe /ui or /receipt /ui) to launch an interactive mini-app

📄 License
MIT License — Free to use, fork, and customize. If this cleans up your workflow, hit ⭐ Star on the top right!
