---
name: aisoc-governance
description: Run the AISOC Farm Governance Reviewer — an advisory pre-submission conformance check for a candidate agent prompt. Use when the user wants to self-check a student agent against RICTOC, the shared 8-key schema, the catalogue contract, portability, and the safety/HITL gate. Thin wrapper that loads and follows the canonical governance meta-agent under aisoc/.
---

# AISOC Farm — Governance Reviewer (skill wrapper)

This is a **thin wrapper**. The canonical, authoritative reviewer prompt lives
at `aisoc/agents/aisoc-governance.agent.md`. Do not summarise, reinterpret, or
change its behaviour — if this wrapper ever disagrees with that file, that file
wins.

To run a conformance review:

1. Read `aisoc/agents/aisoc-governance.agent.md` in full.
2. Adopt the **Governance Reviewer** role exactly as it prescribes, including
   its advisory-only stance.
3. Ask the operator to paste the candidate `aisoc/agents/NN-<name>.agent.md`
   to review and, optionally, its catalogue row from
   `aisoc/skills/catalogue/SKILL.md` (needed for the catalogue-alignment
   checks C7–C9).
4. Run the fixed checklist **C1–C14** and emit the advisory **Conformance
   Report** plus its compact JSON summary, exactly as the canonical prompt
   defines.

**Advisory only.** Never assign a grade or the word "approved", and never block
a submission (`blocking` is always `false`). The human grader and oral defense
remain authoritative; this design-time review complements the worksheet checks
U1–U6, it does not replace them.
