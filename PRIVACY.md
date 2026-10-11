# VibeAds privacy notice

Effective date: 2026-10-11.

VibeAds is a skills-only research and planning plugin maintained by Khadin Akbar. It has no publisher-operated storage service, telemetry endpoint or background synchronization.

For planning, the host processes the brief and evidence the user explicitly supplies for the current task. The plugin does not instruct the host to search unrelated files, memories, chat history or conversation summaries. Local reports are created only when requested. Users control those files and can delete them through their host or file manager.

For connected research, the user authorizes the official Apify CLI, an Apify account and the exact research inputs before execution. Inputs can contain public advertiser names or IDs, keywords, public websites, market/language/date filters and limits. The CLI sends these inputs to Apify. Actors return public ad-library records, keyword estimates or public page metadata. Those records may incidentally contain public personal information, such as an individual advertiser's name. Do not request sensitive personal data, private profiles, customer lists or private account pages. Reports omit contact details and unnecessary identifiers.

Apify stores run inputs, datasets, run metadata and logs under the user's Apify account settings. An Actor can send necessary parts of the research input to its disclosed providers and public source websites. The plugin cannot promise deletion or a fixed retention period for Apify or those providers. Users manage Apify retention and deletion in Apify and should review the current Actor disclosures and relevant provider policies before running research.

Apify authentication is handled by the official CLI. The plugin must not read credential files, enumerate environment secrets, display tokens, place credentials in input JSON or include secrets in reports or support tickets. Provider credentials configured by the Actor owner remain in the remote Actor environment and are not supplied by this plugin.

The assistant host processes prompts, evidence and outputs under its own policies. This notice does not replace that host's policy. VibeAds does not send a copy of user reports to its publisher. If users seek support, send only a sanitized issue description; support platforms handle that submission under their policies.

See [Data flow and third-party privacy policies](skills/ads/references/data-flow.md) for service disclosures. Use [GitHub Issues](https://github.com/khadinakbarlabs/vibeads/issues) for sanitized general questions and [private vulnerability reporting](https://github.com/khadinakbarlabs/vibeads/security/advisories/new) for security concerns. Do not post personal records or credentials. GitHub processes support submissions under its own policies.
