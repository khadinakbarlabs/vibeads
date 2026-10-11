---
name: landing-page-review
description: "Review the fit between an ad's promise and its public landing page, combining supplied page evidence with optional Website SEO Crawler Actor metadata. Use for ad-to-page message match, paid-traffic landing-page checks or conversion-readiness planning. Distinguishes technical findings from visual, form, analytics and performance checks that need separate evidence."
---

# Ad-to-landing-page review

Read [workflow rules](../ads/references/workflow-rules.md), [CLI guide](../ads/references/cli-guide.md), [Actor contracts](../ads/references/actor-contracts.md), [security boundaries](../../SECURITY.md) and the [landing-page checklist](../ads/references/templates/landing-page-review.md).

1. Identify the approved public destination URL, source ad/keyword, campaign objective, target device and promised next step. Reject private/account pages, embedded credentials, localhost, loopback, private-network, link-local and cloud-metadata targets. If public-host safety or redirects cannot be established, prepare a review from supplied evidence without submitting the URL.
2. With approved connected scope and charges, use the Website SEO Crawler Actor with `crawlScope: page-only`, `maxPages: 1`, `maxDepth: 0`, `respectRobotsTxt: true`, direct mode and low concurrency. Multiple URLs need explicit scope/count approval. Do not fetch unrequested related pages, submit forms or change websites.
3. Map the actual fields: HTTP status/redirect, title/meta/H1, canonical/indexability, viewport and issue flags. These support technical and message checks. SEO indexability is not an advertising eligibility or conversion-rate score.
4. Evaluate visible offer/hero/CTA/proof and mobile layout only when page text, screenshots or a user-authorized visual observation are available. A crawler's title and H1 do not reveal its complete visible offer or layout. Mark each missing item `needs_visual_check`.
5. Mark form submission, checkout, consent, analytics, conversion-event delivery and Core Web Vitals `needs_separate_test` unless explicitly observed through an authorized test. `responseTimeMs` is one request's response time, not a Core Web Vitals measurement.
6. Return prioritized fixes with the exact observation, relevance to the ad promise, impact hypothesis, effort, owner and verification step. Use `verified`, `inferred`, `not_tested` or `blocked` per check rather than an invented universal conversion score.

Finish with URL/capture/build provenance and a prelaunch checklist for the advertiser. Do not claim the page is conversion-ready until the missing behavior checks are actually completed.
