# Data flow and external services

The plugin contains instructions and reference files. It has no hosted publisher backend or telemetry. Connected execution uses the separately installed official Apify CLI under the user's explicit authorization. This is local code execution even though the package ships no executable.

| Step | Data/destination | Authority and retention |
| --- | --- | --- |
| Planning | Current task brief/evidence processed by the assistant host | Host policy applies; no research upload |
| Run request | Reviewed public query JSON and CLI authentication sent to api.apify.com | User-authorized account; authentication handled inside the official CLI |
| Actor execution | Selected queries sent by the remote Actor to disclosed providers/public sources | Current Actor disclosure and provider/source terms apply |
| Storage | Input JSON, datasets, run records, logs and summaries in the user's Apify account | Retention/deletion follows Apify account controls; plugin promises no fixed period |
| Collection | Bounded dataset/summary records returned through the CLI to the host | May include incidental public personal identifiers; minimize output |
| Reports | User-requested local artifacts or text in the conversation | No automatic publisher copy, cloud sync or sharing |

## Actor-specific routes to inspect

- **Meta Ad Library:** the selected Actor's public README discloses ScrapeCreators or SociaVault provider-backed retrieval of public Meta records. Only necessary advertiser/search/filter input is sent. Owner-managed provider credentials are remote and are never read or supplied by VibeAds.
- **Google Ads Transparency:** the Actor can start a specialist Apify Ads Transparency Actor in the user's account with separate charges, plus a public-source fallback. Inspect the current provider route and parent/child budget behavior. Ad format filters can cause a larger billable provider sample than the number of parent rows saved.
- **Google sponsored SERPs:** the input contract supports a SerpAPI route or browser route. No user provider-key override is populated. Check the actual route, availability, credits and source scope before a run.
- **TikTok Creative Center, TikTok Ads Library, LinkedIn Ad Library, Pinterest Ads Repository and Snapchat Ads Gallery:** public advertising sources, potentially through Actor-managed retrieval/proxy routes. Confirm current Actor disclosures; do not assume every country, ad or field is covered. Snapchat commercial search covers EU/EEA gallery markets. TikTok Ads Library covers its declared European-country enum. Pinterest uses a narrow date window and small page-boundary sample.
- **Keyword Search Volume API:** DataForSEO Google Ads search-volume service. Sends public phrases and market/language filters; retains source/status on returned metric rows. `free_tier` is a list-size mode and still has request/row charges.
- **Website SEO Crawler:** fetches only the approved public destination, subject to the configured scope, robots rules and any declared proxy route. It does not send private customer/account records or submit forms.

This release verifies public contracts, not the complete network route of a live run. Before connected use, inspect the current README/metadata for the selected build and disclose newly identified providers. Missing destination/cost information means `needs_contract_review`; it is not permission to hide a route or execute first.

## Policies

- [Apify privacy](https://docs.apify.com/legal/privacy-policy) and [Apify terms](https://docs.apify.com/legal/general-terms-and-conditions)
- [DataForSEO privacy](https://dataforseo.com/privacy-policy)
- [SerpAPI legal documents and privacy policy](https://serpapi.com/legal)
- [ScrapeCreators privacy](https://scrapecreators.com/privacy)
- [SociaVault privacy](https://sociavault.com/privacy)

The ScrapeCreators and SociaVault policy pages were verified on 2026-10-11. Review all applicable policies and the current routes before connected execution. Source-platform and assistant-host policies also apply. An accessible draft VibeAds privacy notice does not replace provider policies.
