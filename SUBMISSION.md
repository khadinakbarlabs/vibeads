# Anthropic submission preparation

Prepared against the current [plugin checklist](https://claude.com/docs/plugins/pre-submission-checklist), [submission guide](https://claude.com/docs/plugins/submit), [Directory Policy](https://support.claude.com/en/articles/13145358-anthropic-software-directory-policy) and [Directory Terms](https://support.claude.com/en/articles/13145338-anthropic-software-directory-terms), checked 2026-10-11.

Requested listing title: **VibeAds: Paid Ads Research & Planner**. Identifier: **vibeads**. Publisher shown in the live portal: **Khadin Akbar**. Version: **0.1.0**. The plugin is skills-only and invokes a separately installed CLI for connected research.

## Before submission

1. The user confirmed the exact title, description, capabilities, privacy/terms text and source publication on 2026-10-11. Legal acceptance remains a separate action for the authorized developer.
2. Publish the approved source to [khadinakbarlabs/vibeads](https://github.com/khadinakbarlabs/vibeads). Verify documentationUrl, supportUrl, privacyPolicyUrl and termsOfServiceUrl after the push. Public GitHub Issues support and private vulnerability reporting are configured for the dedicated repository.
3. Validate the final repository commit in the live portal. Resolve blocking findings. Do not treat local schema validation as portal validation or a security scan.
4. Verify connected behavior against the selected builds with a separately approved research account and cost controls. Provide reviewer access through secure portal fields if Anthropic requires it; never package credentials. Run representative prompts in the supported host and report actual results.
5. Answer data-handling questions from the real data flow: selected public query inputs leave the host for Apify; datasets and run inputs persist in the user's Apify account under its controls; public ads may include incidental personal identifiers. No publisher telemetry service or hidden upload is present. Do not claim zero third-party storage or a fixed retention period.
6. Resolve the CLI acknowledgement issue below, have the authorized developer complete legal attestations, and submit only after the user's approval. Confirm the saved source commit/version and the resulting review state. Keep approval, submission, scan, vendor review and publication separate.

## Observed acknowledgement mismatch

The live form at claude.ai/directory/manage/new/plugin, Compliance, on 2026-10-11 requires: “The plugin does not exfiltrate credentials or execute code outside its declared MCP servers.” VibeAds is deliberately a skills-only CLI workflow with no declared MCP server. Its connected research therefore cannot make the literal no-execution assertion. The checkbox was left unchecked. A user's approval of the package does not resolve that factual mismatch. Obtain official clarification that covers this external CLI design before confirming it, or revisit the design with the user's authorization. Do not hide CLI instructions or add a placeholder server to pass the form.

Source publication is authorized. Public URL readback, portal validation and any saved submission identity are recorded separately after they occur. This document is preparation evidence, not a claim of Anthropic approval or directory availability.
