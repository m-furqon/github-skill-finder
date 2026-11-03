# Compatibility Matrix

| Candidate type | Gemini Apps classification | Guidance |
|---|---|---|
| Instruction-only `SKILL.md` with supported references | A, after inspection | Upload and review |
| Skill with optional scripts, core workflow remains instruction-led | B | Remove or separate scripts; rewrite steps |
| Skill requiring local shell execution | C | Use another runtime or create a manual approximation |
| MCP server or daemon | C | Not an uploadable instruction skill by itself |
| Browser automation extension | C or B | Depends on whether the core task can be rewritten |
| API integration requiring secrets and runtime | C or B | Do not embed credentials; use supported integrations |
| Repository inaccessible or file uninspected | U | Do not recommend as verified |

This matrix is a decision aid, not a guarantee. Check current official Google documentation for Gemini Apps behavior.
