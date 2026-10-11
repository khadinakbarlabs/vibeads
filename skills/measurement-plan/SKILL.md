---
name: measurement-plan
description: "Plan conversion measurement, attribution checks and paid-ad experiments before a media test. Use for PPC tracking requirements, UTM planning, CPA/ROAS definitions, lead-quality measurement or creative-test design. Produces a verification checklist and decision rules from supplied context; it does not install tags, collect personal records or claim tracking is working without evidence."
---

# Measurement and experiment plan

Read [workflow rules](../ads/references/workflow-rules.md), [planning math](../ads/references/planning-math.md) and [measurement template](../ads/references/templates/measurement-plan.md).

1. Define one primary business conversion, its qualification rules, value/currency, source of truth, attribution window/timezone and expected conversion lag. Separate clicks, platform-reported conversions, qualified leads and paid customers.
2. Specify events and parameters the advertiser should verify, deduplication strategy, UTM naming, platform-to-analytics/CRM reconciliation and consent requirements. Do not ask for customer-level records; use aggregate metrics expressly supplied for the task.
3. For each event, record current evidence, owner, an authorized verification method, expected count/value and pass condition. An installed tag, screenshot or crawler result alone does not prove delivery, value, deduplication or consent behavior.
4. Define one-variable experiments with a control, variant, primary outcome, budget/exposure, window, lag allowance, minimum useful sample and a decision rule set before looking at outcomes. Use the relevant baseline rates and desired detectable effect when available. Otherwise label the test exploratory; do not invent statistical significance or universal sample thresholds.
5. Calculate CTR, CVR, CPA and ROAS only with consistent denominators and comparable windows. Undefined denominators remain undefined. Report return on spend separately from contribution profitability; do not pool incompatible attribution sources.
6. State blockers before launch: missing conversion verification, unreliable consent, ambiguous value, insufficient creative or lead follow-up. Give the advertiser a concrete path to verify them. This skill prepares a checklist and does not edit tags, accounts or code.

Return a measurement contract and a review cadence. No automatic scheduler is created. If the user wants recurring work, prepare a separate proposal specifying scope, costs and notification intent for approval through the host's supported scheduling interface.
