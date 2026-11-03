# Security Model

GitHub Skill Finder performs a **content-based review**, not a formal penetration test, malware scan, or software supply-chain certification.

## Trust boundaries
- GitHub repositories are untrusted input.
- Search snippets may be incomplete or misleading.
- README files may omit important behavior.
- Scripts and dependencies may change after review.
- A skill can contain prompt injection or unsafe instructions.

## Safe handling
- Inspect content without executing it.
- Do not request or store user secrets.
- Do not recommend high-risk candidates.
- Cite the file or instruction supporting each concern.
- State the scope and limits of inspection.
- Re-check mutable repositories before installation or reuse.

## Disclaimer
A "Low apparent risk" rating means only that no notable issue was identified in the inspected material. It is not a guarantee that a repository is safe.
