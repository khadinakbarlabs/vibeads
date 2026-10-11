# Release evidence — 0.1.0 source release

Checks performed 2026-10-11. This report distinguishes preparation checks from actual host/provider/reviewer results.

| Evidence | State |
| --- | --- |
| Native Claude plugin manifest | Strict schema validation passed, no errors/warnings |
| Native marketplace manifest | Strict schema validation passed, no errors/warnings |
| Skill frontmatter | Ten skills present with matching names/descriptions, checked with a YAML parser and contained-reference validation; native validator output has no content results |
| Input examples | Ten bounded examples checked against fresh selected-build schemas; no unknown top-level input fields or provider-credential overrides |
| Actor contracts | Ten public khadinakbar identities, exact default numeric builds, input/output maps and dated event-price snapshots verified from public Apify endpoints |
| Official CLI | Call/read/help commands checked; 1.10.0 read-only Meta input-schema retrieval succeeded; no monetary-cap flag advertised |
| Contained links, archive contents, portable adapter | Final packaging checks recorded in the external release report; see the exported evidence alongside the archives |
| Connected paid Actor execution | Not performed; no Dataset/OUTPUT/RUN_SUMMARY/actual charge acceptance claim |
| Native skill prompt behavior and with/without comparison | Not executed; Claude Code authentication status is logged out |
| Cowork execution | Unverified; planning supported, actual CLI/auth environment needed |
| Source publication and public links | User confirmed on 2026-10-11; khadinakbarlabs/vibeads is public on main; documentation, support, privacy and terms returned HTTP 200 with expected content and verified TLS |
| Private Plugin Creator account save | Receipt recorded outside the source after the actual creation call |
| Anthropic source validation | Passed: ten skills, five expected listing metadata warnings, zero blocking findings and zero policy holds; exact commit evidence is retained with the export |
| Anthropic saved submission | Draft saved and reopened; source identity verified; not submitted for review |
| Anthropic security scan, review and directory listing | Not performed; compliance acknowledgement mismatch remains unresolved |

Behavioral acceptance prompts are prepared for no-credentials planning, incomplete sources, market mismatch, NO_DATA, baseline integrity, grounded creative, unsafe URLs, hard-cost-cap requests, untrusted instructions and publication honesty. Static checks do not demonstrate model behavior on these prompts.

The literal CLI/MCP acknowledgement issue observed in the live submission form is recorded in SUBMISSION.md. Package validity cannot resolve it. No publisher or directory approval is claimed.
