# GitHub Skill Finder v2.0

**Discover. Verify. Audit. Adapt. Organize.**

GitHub Skill Finder is a Gemini Apps Skill designed to help users discover AI agent skills on GitHub, verify their contents, assess Gemini Apps compatibility, review security risks, adapt portable instructions, and organize selected skills into a collection.

> This project is an instruction-based Skill for Gemini Apps. It does not automatically install arbitrary GitHub repositories, execute downloaded scripts, or guarantee that third-party skills are safe.

## What it does

- **Multi-category discovery** — research, coding, data, design, business, education, productivity, cybersecurity (defensive/authorized), science, writing, and more.
- **Repository verification** — locate and inspect the actual `SKILL.md`, README, license, dependencies, and maintenance evidence.
- **Gemini compatibility assessment** — classify candidates as likely compatible, compatible with adaptation, not directly compatible, or unverified.
- **Security review** — inspect instructions and available files for credential exposure, suspicious scripts, exfiltration, destructive actions, and excessive permissions.
- **Duplicate detection** — identify likely duplicate or overlapping repositories and explain the evidence.
- **Cross-platform adaptation** — prepare a Gemini Apps-oriented instruction-only version when a source skill can be safely adapted.
- **Collection planning** — organize selected skills into a proposed collection with clear names, scopes, and overlap warnings.
- **Evidence-based ranking** — score relevance, compatibility, documentation, maintenance, security posture, and license clarity.

## Repository structure

```text
github-skill-finder-v2/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── .gitignore
├── .github/
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md
│       └── skill_request.md
├── docs/
│   ├── COMPATIBILITY-MATRIX.md
│   ├── SECURITY-MODEL.md
│   └── WORKFLOWS.md
└── skills/
    └── github-skill-finder/
        ├── SKILL.md
        └── references/
            ├── COMPATIBILITY-CHECKLIST.md
            ├── SEARCH-PLAYBOOK.md
            ├── SECURITY-AUDIT.md
            ├── SCORING-MODEL.md
            └── GEMINI-ADAPTATION.md
```

## Install in Gemini Apps

1. Open [Gemini](https://gemini.google.com/).
2. Open **Customize** → **Skills**.
3. Choose **Create** → **Upload**.
4. Upload the folder `skills/github-skill-finder/` or a ZIP containing that folder with `SKILL.md` inside it.
5. Review the imported Skill and save it.
6. Enable the Skill if needed.

The exact interface and upload limits may vary by account, region, and product rollout. Check current official Google documentation if the menu differs.

## First test prompt

```text
Use GitHub Skill Finder v2.0 to find 10 high-quality GitHub agent skills
across different categories that can be used in Gemini Apps.

For each candidate:
- verify the repository and exact SKILL.md path;
- inspect the actual skill instructions;
- assess Gemini Apps compatibility;
- review dependencies, license, maintenance evidence, and security risks;
- detect duplicates or substantial overlap;
- score and rank the results;
- provide repository and SKILL.md links.

Do not invent repositories, claim untested installation, or label a
skill directly installable unless its requirements support that conclusion.
```

## Important limitations

- Gemini Apps Skills are instruction bundles, not arbitrary executable plugins.
- A GitHub repository containing `SKILL.md` is not automatically compatible with Gemini Apps.
- Skills requiring local shell execution, internet-enabled scripts, MCP servers, daemons, browser automation, or unsupported APIs may need another runtime or adaptation.
- This Skill can inspect and reason about content available to Gemini; it cannot guarantee a complete malware audit.
- It does not execute third-party code or install external repositories automatically.
- Search quality depends on live web access and the capabilities available in the user's Gemini account.

## Project status

Version: **2.0.0**  
Target platform: **Gemini Apps**  
Scope: **All categories**  
Mode: **Discovery + compatibility assessment + adaptation guidance + collection planning**

## License

See [LICENSE](LICENSE). The license applies to this project’s original files. It does not grant rights to third-party repositories discovered by the Skill.
