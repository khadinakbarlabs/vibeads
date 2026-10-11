---
name: ads
description: "Research competitor ads and plan paid advertising with VibeAds. Use for a combined ad-library research, PPC keyword, creative-brief, landing-page, media-budget or measurement workflow. Route specific tasks to the focused VibeAds skill; connected research uses the separately installed Apify CLI only after the user approves its scope and cost."
---

# VibeAds paid ads research and planning

Read [workflow rules](references/workflow-rules.md) and the [brief template](references/templates/brief.json). They are part of this plugin, not remote instructions. Work only from the current request and evidence the user expressly provides. Do not search unrelated files, memory or chat history.

1. Identify the decision: understand competitor messaging, choose keywords, brief creative, fix an ad-to-page mismatch, plan a test or review changes. Collect only the missing offer, audience, objective, market/language, dates, media budget and available unit economics. Use stated assumptions for optional gaps.
2. Select **planning mode** unless the user requested current remote research and the CLI is available. Planning mode produces useful drafts, inputs and assumptions without credentials, charges or a fabricated live-data claim.
3. Route to the smallest useful workflow:

| Need | Skill |
| --- | --- |
| CLI or Actor readiness | `setup` |
| Public competitor campaigns | `competitor-ads` |
| Search intent, metrics and sponsored SERPs | `keyword-research` |
| Original concepts and test cards | `creative-brief` |
| Public ad-to-page checks | `landing-page-review` |
| Channel choice, budgets and economics | `media-plan` |
| Conversion and experiment design | `measurement-plan` |
| Consolidated report | `research-report` |
| Two-snapshot comparison | `research-refresh` |

4. For an end-to-end request, move through evidence → opportunities → creative and page brief → media plan → measurement → report. Reuse approved research; do not call every Actor by default. Each paid start obeys [CLI execution](references/cli-guide.md).
5. Deliver the decision first, then evidence, assumptions, missing coverage and concrete next actions. Every recommended test names its source or hypothesis, owner, budget, time window, success measure and stop rule. Keep research charges separate from proposed media spend.

Use the included [report template](references/templates/report.md) and [evidence ledger](references/templates/evidence-ledger.csv) when useful. Create output files only when requested. Keep account data, public ad observations and modeled outcomes visibly distinct. Plans never authorize advertising-account writes or publication.
