---
name: keyword-research
description: "Plan PPC keywords using user-supplied seed phrases, Google sponsored-result research and the publisher's Keyword Search Volume API Actor. Use for paid-search keyword research, CPC estimates, search-intent clusters, match-type proposals or negative keywords. Separates planning estimates and NO_DATA from observed account performance."
---

# PPC keyword planning

Read [workflow rules](../ads/references/workflow-rules.md), [Actor contracts](../ads/references/actor-contracts.md), [CLI guide](../ads/references/cli-guide.md), [keyword template](../ads/references/templates/keywords.csv) and [planning math](../ads/references/planning-math.md).

1. Define the offer, conversion, target geography/language and first test's economic boundary. Start from phrases supplied by the user or visible in approved public ad evidence. Generated ideas are hypotheses until researched. The metrics Actor measures known phrases; it does not discover a complete keyword universe.
2. Deduplicate, cluster and propose a small list across brand, competitor, high-intent category, use case and problem-aware phrases. Competitor trademarks and their landing pages need advertiser review before using them in ads. Do not mix brand/non-brand results or language markets.
3. For approved connected research, use `keyword-search-volume-api` with a focused list, explicit geography/language and `free_tier` size mode. This mode still incurs charges. Inspect current request-plus-row pricing; even `NO_DATA` rows may be billable. Keep provider-credential override fields absent.
4. Optionally research Google sponsored results with `google-ads-scraper` only for selected queries after its additional charge is approved. Its lowercase country enum differs from other Actors; unsupported markets must not be silently substituted.
5. Accept metrics only when a row's `status` is `OK`, with source and `fetchedAt`. Preserve `NO_DATA`, null fields and partial failures. Null volume or CPC is unknown, not zero demand or free traffic. Do not multiply estimated monthly query volume into a guaranteed acquisition forecast.
6. Produce intent clusters, suggested exact/phrase starting tests, negative-keyword candidates, rationale, estimated CPC/bid range where supplied, capture date and confidence. A term is a candidate negative until conversion and query context support exclusion.
7. For an optional click/conversion scenario, show budget ÷ assumed CPC and clicks × assumed conversion rate, with low/base/high assumptions. Forecasts are conditional. Use the advertiser's account history where supplied; library estimates do not replace it.

Deliver a prioritized test list and explicitly mark missing metrics, policy/trademark review, measurement requirements and scope gaps. Do not change keywords or advertising accounts.
