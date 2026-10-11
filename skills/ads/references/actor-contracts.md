# Verified public Actor contracts

These are the publisher's ten selected public Actors. IDs, default build pins, schemas, output-field maps and event-price snapshots were read from public Apify metadata/build endpoints on 2026-10-11. They establish contracts, not runtime success or cloud availability. Refresh before paid use.

| Source | Exact Actor ID | Numeric build pin | Bounded example | Coverage and limitations |
| --- | --- | --- | --- | --- |
| Meta Ad Library | `2yvvGyBDQXi41nPrW` | 1.0.8 | [Input](inputs/facebook-ads-library-scraper.json) | One requested country; provider-backed sample. Default latest remains 1.0.8; separate October 10 fix tags are not promoted or treated as validated. |
| Google Ads Transparency | `dCA5Hpf4BCQX094ZD` | 1.5.10 | [Input](inputs/google-ads-transparency-scraper.json) | Copy, landing page and platform fields can be absent. Public-source regions differ from requested filters. Specialist child Actors incur separate charges, including filtered provider records. |
| Google sponsored search | `w9R2Ra2aW9iROZcNW` | 1.0.16 | [Input](inputs/google-ads-scraper.json) | Query/device/market/time-specific sponsored results. No stable ad ID; composite matches are weak. Country uses a restricted lowercase enum. Live ad-found price differs from prose in input schema; use pricing metadata. |
| TikTok Creative Center | `cSmKlcb02KBxMla6X` | 1.0.28 | [Input](inputs/tiktok-ads-scraper.json) | Curated Top Ads sample, not a complete advertiser inventory. CTR/cost tiers are source-disclosed relative metrics, not account ROAS. No landing URL field in this contract. |
| TikTok Ads Library | `x5x84HE8Hq7EJ9VmS` | 1.1.6 | [Input](inputs/tiktok-ads-library-scraper.json) | EEA/UK/Swiss library countries only, exactly as input enum. US not supported. Optional public audience fields are not privately measured conversions. |
| LinkedIn Ad Library | `f4XR9mQaMv1JNMh71` | 0.2.9 | [Input](inputs/linkedin-ads-scraper.json) | Requested public library scope and dates; accountOwner/payer/keyword modes differ. Detail enrichment creates additional events. No landing URL field in this contract. |
| Pinterest Ads Repository | `oKsJ4mO6RAVbvcrnz` | 1.0.3 | [Input](inputs/pinterest-ads-library-scraper.json) | Supported public-repository markets, date window at most 31 days; repository page-boundary cap is 24. No landing URL field in this contract. |
| Snapchat Ads Gallery | `pNrBHdXl6lOdDMiLu` | 0.1.7 | [Input](inputs/snapchat-ads-scraper.json) | Commercial search uses EU/EEA gallery coverage. VibeAds does not select creator/political mode. Source capture timestamp may be absent; use labeled run-collection time. |
| Google Ads keyword estimates via DataForSEO | `B7Wq9VHcVFdfNqNBI` | 0.1.7 | [Input](inputs/keyword-search-volume-api.json) | Known keyword metrics, not idea discovery. NO_DATA/null unknown; free_tier is a 25-keyword size mode with request and row charges. |
| Public landing-page metadata | `f0PPU2rWRKUBwAfeZ` | 0.2.5 | [Input](inputs/website-seo-spider.json) | One approved public page by default. Crawl evidence is not form/analytics/consent/Core Web Vitals or conversion-rate evidence. |

Full field maps, default memory/start units and current-as-of event prices are in [contracts JSON](actor-contracts.json). The input examples are sample queries, not recorded runs. Replace targets only within user-approved scope; do not execute the examples automatically.

## Cost details

- Latest metadata is the pricing source. The Google sponsored-search input schema still mentions an older per-row price; the verified current event metadata is different. Do not use descriptive prose as a billing quotation.
- Keyword metrics can incur both a successful provider-batch event and a charge for every saved metric row, including NO_DATA. free_tier refers to list size, not a free price.
- Google Transparency can use separately billed specialist child runs. Format filters can bill more child/provider records than parent rows. The parent cap alone does not cap the entire bill. Inspect actual provider and combined child-budget evidence before requesting approval.
- Default memory varies; TikTok Actors are configured for 4096 MiB and may have four start-event units where start pricing is per GB. Platform charges and unknown defaults stay separate from event-only estimates.
- CLI item/page limits and timeout do not constitute a hard monetary cap. Do not invent a CLI charge flag.

## Interpretation

Do not create a field absent from the native output. A mapping names a possible returned field, not a guarantee it is populated. Preserve source IDs/dates/status; label collection-time substitutions. Do not conflate public ranges/tier indicators, source status, page metadata, private account performance and modeled outcomes. Missing summaries or failed sources remain unverified/failed rather than zero.
