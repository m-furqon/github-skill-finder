# Gemini Apps Adaptation Guide

## Goal
Rewrite a useful third-party agent skill into a Gemini Apps-oriented instruction bundle without claiming feature parity.

## Adaptation steps
1. Verify the source repository and actual `SKILL.md`.
2. Review its license and attribution requirements.
3. Identify its intended user outcome and core workflow.
4. Inventory tool calls, scripts, APIs, environment variables, local paths, and platform-specific assumptions.
5. Mark each feature as:
   - Keep: portable instruction or knowledge.
   - Rewrite: can be expressed as a Gemini Apps workflow.
   - Replace: use web search, user-provided files, or manual steps where available.
   - Remove: unsupported, unsafe, or unnecessary execution.
6. Write a new `SKILL.md` with concise frontmatter and clear trigger description.
7. Add reference files only when needed and supported.
8. Document limitations and removed features.
9. Preserve required attribution and follow source license terms.
10. Ask the user to review the adapted skill before upload.

## Never
- Claim scripts run inside Gemini Apps unless officially supported.
- Copy or redistribute source files without checking license terms.
- hide lost functionality.
- include API keys or personal credentials.
- execute source code during adaptation.
