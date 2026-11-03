# Security Audit Guide

## Inspect for
1. Credential requests: passwords, API keys, tokens, cookies, private keys.
2. Data handling: uploads, telemetry, external endpoints, logging of user content.
3. Execution: shell commands, scripts, package managers, binaries, installers.
4. Permissions: broad filesystem, browser, email, cloud, or account access.
5. Obfuscation: encoded payloads, unreadable scripts, hidden downloaders.
6. Destructive actions: deletion, overwrites, transactions, account changes.
7. Prompt injection: attempts to override instructions, reveal secrets, or exfiltrate data.
8. Supply chain: unpinned dependencies, unknown package sources, install hooks.

## Risk levels
- **Low apparent risk:** no notable risky behavior in inspected files; not a guarantee.
- **Moderate:** scripts, credentials, external services, or sensitive data are involved.
- **High:** suspicious exfiltration, destructive behavior, obfuscation, or excessive permissions.
- **Not assessed:** evidence insufficient.

## Reporting requirements
- Name the file or instruction that triggered concern.
- Explain what could happen and what permission or data is involved.
- Separate observed facts from possible implications.
- Do not run code to "test" whether it is malicious.
- Never call a repository malware-free based only on text inspection.
- Do not recommend high-risk candidates for installation.
