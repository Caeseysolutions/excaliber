# CHANGELOG — Caeseysolutions/excaliber
# File: CHANGELOG.md
# Repo: https://github.com/Caeseysolutions/excaliber
# Dashboard URL: https://caeseysolutions.github.io/excaliber
# Access code: exec2026

---

## VERSION REGISTRY

| Version | Date | File deployed | Commit message | Deployed by |
|---|---|---|---|---|
| v2 | 2 Apr 2026 | excalibur_dashboard_v02apr2026.html → index.html | excaliber dashboard v2 - QA agent RULE 13 + April 2026 update | Kristof |
| v1 | Mar 2026 | excalibur_dashboard (2).html → index.html | Initial deploy | Kristof |

---

## v2 — 2 April 2026
**File:** excalibur_dashboard_v02apr2026.html → upload as index.html
**Commit message:** `excaliber dashboard v2 - QA agent RULE 13 + April 2026 update`

### What changed
- Fix: QA Gate Agent prompt — RULE 13 added (JS-escaped multilingual translation bleed detection)
- Fix: QA checklist context date updated March 2026 → April 2026
- Root cause documented: French rv2 string delivered in Dutch NL block on drivealert.eu — passed grep checks because JS \\' escape prevented pattern matching
- RULE 13 mandates: unescape JS strings before scanning for language bleed using marker word lists (EN/NL/FR/DE)

---

## v1 — March 2026
**File:** excalibur_dashboard (2).html → uploaded as index.html
**Commit message:** Initial deploy

### What's in the dashboard
- 9 tabs: Dashboard, Battle Plan, Agents, Health, Income, Security, Prompts, Assets, Correction
- 15 agent prompts (Master, Scaling, Battle Plan, Programming, Marketing, Strategy, Finance, Outreach, Security, Legal, Content, QA Gate, Adaptive Learning, Correction, Opportunity Scout)
- Income tracker (€0/€200 target)
- Security scanner (paste-and-scan)
- Activity log
- Correction log
- All agent prompts copy-ready

---

## DEPLOY INSTRUCTIONS — READ EVERY TIME

### Files in this repo
| File | Purpose | Touch? |
|---|---|---|
| index.html | Dashboard — the actual page | YES — each version |
| CHANGELOG.md | Version registry | YES — update before each deploy |
| robots.txt | Blocks search engines (dashboard is private) | NO — never touch |
| .nojekyll | GitHub Pages Jekyll bypass | NO — never touch |

### How to deploy a new dashboard version
1. Go to: https://github.com/Caeseysolutions/excaliber
2. Click: Add file → Upload files
3. Upload: the new dashboard HTML file + updated CHANGELOG.md
4. **IMPORTANT: rename the HTML file to index.html before uploading**
   - Your download will be named: excalibur_dashboard_v[date].html
   - GitHub needs it named: index.html
   - Rename on your computer before dragging into GitHub
5. Commit message: see VERSION REGISTRY above
6. Commit directly to main

### How to name the next version
- File to download from Claude: excalibur_dashboard_v[DDmonyyyy].html
- Rename to: index.html before uploading to GitHub
- Commit message format: `excaliber dashboard v[N] - [one line description]`
- Add row to VERSION REGISTRY table above

### ⚠️ MISFIRED DEPLOY WARNING
If you accidentally upload the wrong file (e.g. drivealert index.html into excaliber):
1. Go to repo → click index.html → click pencil icon → this is the ONLY time pencil is ok
2. Actually: better to just re-upload the correct file via Upload Files
3. The correct excalibur dashboard file is always named: excalibur_dashboard_v[date].html

### Current live version
**v2** · deployed 2 April 2026 · QA Agent RULE 13 included
