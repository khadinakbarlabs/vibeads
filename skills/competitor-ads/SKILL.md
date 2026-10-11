---
name: competitor-ads
description: "Research public competitor ads with Meta Ad Library, Google Ads Transparency, TikTok Creative Center or Ads Library, LinkedIn, and market-supported Pinterest or Snapchat sources. Use for competitor ad research, ad-library analysis, ad messaging, offer patterns or creative gaps. Delivers a sourced matrix, not competitor spend or ROAS estimates."
---

# Competitor ad research

Read [workflow rules](../ads/references/workflow-rules.md), [Actor contracts](../ads/references/actor-contracts.md), [CLI guide](../ads/references/cli-guide.md) and the [competitor matrix](../ads/references/templates/competitor-matrix.csv).

1. Confirm the competitors, exact public advertiser identities or domains, decision, market/language and capture window. Start with a small named set. Resolve ambiguous company names before attributing ads; matching brand words alone is insufficient.
2. Choose only the requested platforms. Meta serves Facebook/Instagram library evidence; Google Transparency serves disclosed creatives and dates; Google sponsored SERPs are a separate query-specific source. TikTok Creative Center is a curated sample and differs from the Ads Library. LinkedIn, Pinterest and Snapchat may have narrower public-market coverage. The TikTok Ads Library Actor has a European-country enum: a US request cannot be executed as DE. Propose the US Creative Center source as a different source with explicit approval if useful.
3. In planning mode, create the request and matrix schema from supplied evidence. For connected mode, follow `setup`; run only approved Actors/inputs/builds. Do not expand to related brands, regions or paid enrichment on your own.
4. Collect using the same run's dataset and available `OUTPUT`/`RUN_SUMMARY`. Keep per-platform status: `complete`, `partial`, `failed`, `not_requested` or `unverified`. Do not merge a failed source into zero ads.
5. Normalize records using the field map in [contracts JSON](../ads/references/actor-contracts.json). Preserve platform, advertiser identity, ad ID, source URL, capture date, observed run dates/status, country/filter scope, copy summary, CTA, format and landing URL. Deduplicate by platform plus stable ad ID; otherwise retain a labeled weak match.
6. Cluster patterns into offer, customer problem, proof, hook, CTA, format and funnel destination. Count patterns only within the sampled records and state the denominator. Separate direct facts from inferred customer intent. Public impression/spend ranges, when present, retain their exact meaning and source; never create general account-performance claims.
7. Return three to five original opportunities with evidence IDs, alternative explanations and an experiment that could validate each. Long-running ads are longevity observations, not proven winners. Keep excerpts short and do not download or copy protected creative assets.

Finish with coverage, failures, missing evidence, run/build provenance, verified charges or charge uncertainty, and a clear recommendation for the next planning step. An incomplete provider run is not a reason to start a new paid attempt without authority.
