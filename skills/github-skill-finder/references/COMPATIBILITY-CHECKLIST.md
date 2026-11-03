# Gemini Apps Compatibility Checklist

Use this checklist before classifying a repository as uploadable to Gemini Apps.

## Evidence
- [ ] Repository page opened.
- [ ] Exact `SKILL.md` located and opened.
- [ ] Supporting files identified.
- [ ] README and setup instructions reviewed.
- [ ] License status checked.
- [ ] Maintenance evidence checked.

## Runtime requirements
- [ ] Core workflow is expressed as instructions.
- [ ] No essential local shell or code execution.
- [ ] No essential internet-enabled script.
- [ ] No essential CLI, daemon, MCP server, or browser automation.
- [ ] No required API integration unavailable to Gemini Apps.
- [ ] Required reference files can be uploaded.
- [ ] File formats and size limits checked against current official documentation.

## Classification
- **A — Likely compatible:** instruction-led, supported files, no unsupported runtime.
- **B — Compatible with adaptation:** useful workflow can be rewritten safely.
- **C — Not directly compatible:** essential runtime or external action is unsupported.
- **U — Unverified:** insufficient evidence.

A `SKILL.md` file alone does not prove Gemini Apps compatibility.
