---
name: research-refresh
description: "Compare two explicitly supplied paid-ad research snapshots and plan the next review. Use for competitor-ad changes, new creative or offer patterns, keyword estimate changes or recurring research planning. Matches stable IDs and scope, preserves incomplete coverage and never schedules work or starts new paid research without the user's authorization."
---

# Research comparison and next review

Read [workflow rules](../ads/references/workflow-rules.md) and [comparison template](../ads/references/templates/research-comparison.md).

1. Use the two snapshots the user expressly provides for this task. Compare platform, advertiser identity, market/language, date/filter scope, selected build, source/provider and record limits before comparing results.
2. Match by platform plus stable ad ID. If absent, use a labeled weak composite match and avoid definitive additions/removals. Handle duplicate cards/variants separately from duplicate ads.
3. Classify stable, new in sample, changed, explicitly inactive or missing in sample. An ad absent from a later sample is not proven stopped. Only an explicit source status supports inactive/stopped; a partial, failed or narrower run cannot establish removal.
4. Compare aggregate patterns with consistent denominators. Explain changes in filters, geography, caps, providers or schemas before interpreting market changes. Search-volume/CPC comparisons need the same market, language, source and capture window; changing estimates are not measured account performance.
5. Keep the last complete, comparable baseline intact. Show a new partial snapshot as partial and do not overwrite or advance the baseline. Valid partial observations can still be reported with their limitations.
6. Return changed evidence, possible implications, alternative explanations and next creative/keyword tests. If a refresh is needed, prepare the bounded Actor input and price request through `setup`; do not start or retry paid work from a comparison alone.
7. If the user requests ongoing monitoring, propose exact interval, targets, limits, maximum additional spend mechanism, owner, failure handling and notification criteria. No background task exists until the user explicitly authorizes and the host actually creates one. Stay quiet on unchanged/non-actionable states unless periodic status is requested.

The output is a comparison or monitoring proposal. Do not claim a monitor was created, a baseline advanced or an ad stopped unless that state is verified.
