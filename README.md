# VibeAds: Paid Ads Research & Planner

Research competitor ads. Find useful PPC keywords. Build a media plan you can review and use.

VibeAds is a skills-only plugin for paid advertising research and planning. It helps founders, agencies and marketing teams turn public ad-library records, keyword estimates and landing-page evidence into a competitor brief, original creative concepts, a budgeted campaign plan and a measurement checklist.

## What you get

- **Competitor ad research:** compare hooks, offers, calls to action, creative formats and destinations across Meta, Google, TikTok and LinkedIn. Pinterest and Snapchat research are available where their public libraries cover the requested market.
- **PPC keyword planning:** cluster phrases by commercial intent, inspect search volume and CPC estimates, propose match types and negative-keyword candidates, and review current Google sponsored results.
- **Creative briefs:** build original hooks, copy directions and production briefs, with a source or a clearly stated hypothesis for each concept.
- **Landing-page review:** connect the ad promise to the destination and separate crawler findings from checks that need visual or measurement evidence.
- **Media plans:** choose channels that fit the objective and economics, allocate an explicit budget, model downside scenarios and define stop rules.
- **Measurement and reports:** define conversion events, attribution checks and experiments; deliver a concise report with a source ledger and meaningful coverage limits.
- **Research refresh:** compare two explicitly supplied snapshots using stable IDs and matching markets; distinguish new ads from ads missing in an incomplete sample.

## Try these prompts

1. “Research these three competitors in the United States on Meta and Google. Give me the recurring offers, landing-page patterns and five original creative hypotheses. Prepare the Apify inputs and show the research cost before starting.”
2. “Plan a 30-day Google and Meta test for my SaaS with a $1,500 media budget. Our first-month contribution per customer is $120. Show budget totals, break-even assumptions, a creative brief and a measurement checklist. Use planning mode; do not start research runs.”
3. “Use the public ad records I supplied to prepare a competitor research report. Label missing markets and dates, cite each recommendation, and do not infer ROAS from ad longevity.”
4. “Compare these two research snapshots for the same competitors and market. Show new and changed ads, then recommend which creative hypotheses to review next.”

## Skills

| Skill | Result |
| --- | --- |
| `/vibeads:ads` | A routed, end-to-end research and planning workflow |
| `/vibeads:setup` | CLI readiness and a reviewed, bounded research request |
| `/vibeads:competitor-ads` | A sourced competitor-ad matrix |
| `/vibeads:keyword-research` | Intent clusters and PPC test candidates |
| `/vibeads:creative-brief` | Original creative concepts and test briefs |
| `/vibeads:landing-page-review` | Ad-to-page checks and prioritized fixes |
| `/vibeads:media-plan` | Channel allocation, economics and rollout plan |
| `/vibeads:measurement-plan` | Conversion, attribution and experiment checklist |
| `/vibeads:research-report` | A decision-ready report with an evidence ledger |
| `/vibeads:research-refresh` | An honest comparison of research snapshots |

## Installation and supported surfaces

Install from the public source in Claude Code:

```text
/plugin marketplace add khadinakbarlabs/vibeads
/plugin install vibeads@vibeads-marketplace
```

For a local Claude Code session, load this folder using the official plugin flag:

```sh
claude --plugin-dir /absolute/path/to/vibeads
```

This package contains Markdown skills, JSON reference data and templates, an original SVG icon and policy documents. It has **no bundled executable, MCP server, hook, agent, automatic installer or background scheduler**. Claude Code provides the shell and local-file capabilities; every requested action remains subject to the host's permissions.

Connected research requires the separately installed official **Apify CLI 1.10.0**, a user-authorized Apify login and sufficient account credits. Installation is a user setup step, never an action triggered by loading a skill. See the [CLI guide](skills/ads/references/cli-guide.md). If the host has no usable CLI, VibeAds prepares inputs and works from public evidence or planning assumptions expressly supplied for the task. Browser chat is a planning surface; connected execution in Cowork depends on its actual CLI and authentication environment and is not verified by this release.

## Data, credentials and charges

With permission to run connected research, VibeAds instructs Claude to run the official Apify CLI against the ten public Actors listed in [Actor contracts](skills/ads/references/actor-contracts.md). The CLI contacts **api.apify.com** using the account the user explicitly authorizes. The plugin does not read the CLI's credential store, inspect environment secrets or ask for tokens in chat. The user completes login directly in the official CLI.

Research sends only the reviewed input JSON: public advertiser names or IDs, public domains and URLs, keywords, market/language/date filters and result limits. Apify stores those inputs and the resulting datasets, run records and logs in the user's account. The selected Actors may use provider services, public ad libraries and public websites to retrieve the requested information; the provider disclosures and privacy links are in [Data flow](skills/ads/references/data-flow.md). Provider routes can change, so check the current Actor contract before a connected run.

VibeAds has no publisher-operated data service, telemetry or automatic cloud sync. It only instructs the host to read the plugin's own references and process evidence expressly supplied for the current task. Local output files are created only when the user asks for them. Do not supply customer-level exports, credentials, private account pages or unrelated conversation data.

**Actor research can cost money.** The plugin itself is free; Apify's event charges, platform usage and applicable provider charges are separate. The input mode named `free_tier` on the keyword Actor is a size limit, not a promise of a free run. Each start requires approval of the named Actors, exact inputs, limits, event-price estimate and account. The tested CLI exposes no per-call monetary-cap flag; item limits and timeout are not a guarantee of a maximum total charge. If a hard cap is required, verify a platform-enforced limit before execution or remain in planning mode.

## Evidence and practical limits

Public ad libraries are samples, and their geography and date coverage differ. Ads may be missing because of filters, library coverage, rate limits or provider failures. A finished Apify run alone does not establish complete results: check its dataset, `OUTPUT`, `RUN_SUMMARY`, captured build and charges. Missing summaries are reported as unverified. VibeAds never presents missing data as zero competitor activity.

Public ad presence and duration do not establish spend, conversions, profitability or ROAS. Keyword CPC and volume are planning estimates. The landing-page crawler reports technical and page metadata; it does not test form submission, consent, analytics, conversion rate or Core Web Vitals. Media plans and creative drafts need the advertiser's review and are not forecasts or performance guarantees.

VibeAds does not launch ads, change bids or budgets, purchase media, publish creative or mutate an advertising account. Plans for sensitive or regulated categories require the advertiser's current policy and legal review before use. It does not copy competitor assets or fabricate testimonials.

## Review and release status

Version 0.1.0 is the publisher-approved source release. Local package checks and public Actor contract checks passed; paid Actor execution and native prompt behavior remain unverified. Anthropic portal validation, security scanning, review and directory availability are separate states. See the [release checks](RELEASE-CHECKS.md) and [submission notes](SUBMISSION.md).

[Privacy](PRIVACY.md) · [Terms](TERMS.md) · [Support](SUPPORT.md) · [Security](SECURITY.md) · [Research and attribution](RESEARCH.md)
