---
description: Run the AISOC Farm Governance Reviewer on a candidate agent prompt (advisory self-check)
---

Adopt the role defined in the AISOC Farm Governance Reviewer below. Follow it
exactly, including its advisory-only stance and its **Conformance Report**
output. This is the canonical reviewer prompt — do not summarise, reinterpret,
or skip any of its C1–C14 checks.

After loading it, ask the operator to paste the candidate
`aisoc/agents/NN-<name>.agent.md` to review (and, optionally, its catalogue row
from `aisoc/skills/catalogue/SKILL.md` for the alignment checks C7–C9), then
emit the advisory Conformance Report. Never assign a grade or block a
submission — the human grader and oral defense remain authoritative.

@aisoc/agents/aisoc-governance.agent.md
