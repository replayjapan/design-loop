---
name: design-loop
description: Research relevant UI patterns before substantive design choices, then review the implemented page at desktop and phone widths. Use for interface, navigation, responsive layout and interaction work; skip a full research loop for a mechanical copy or token change.
---

# Design Loop

Use the user's task and the existing product as the brief. Inspect the relevant
page or flow, existing components and design constraints first. Keep the scope
proportionate; do not replace the user's product with a generic redesign.
For each requested element, consider the user need it serves and its effect on
spacing, hierarchy and the surrounding flow. Do not pile every suggestion into
the interface without evaluating the result. If an addition conflicts with the
user's goals or makes the layout crowded, explain the conflict and propose a
simpler arrangement before building. Do not silently omit explicit requirements;
resolve material conflicts with the user while continuing unaffected work.

## Before choosing a design

Return to this research step for each new UI request before building. When the
user names a research source, such as Mobbin, keep using it for each relevant UI
decision until the user changes that instruction. One initial lookup does not
satisfy a standing instruction for later decisions. Previously inspected evidence
may support a decision it directly answers; identify that connection and research
new questions instead of treating the first lookup as blanket coverage.

Identify the specific decision that needs evidence. Use available relevant tools:
Mobbin for comparable flows, an installed frontend-design skill for implementation
guidance, and web/docs for unfamiliar interaction or accessibility constraints.
Absent a user requirement, these are optional capabilities, not dependencies to
install. Start with a small set of relevant references and stop when they answer
the decision. Do not collect
screenshots or make tool calls merely to meet a quota.

Write a short design brief in the reply or an authorized planning location:

- User task, constraints and the UI decision being made.
- Relevant sources, with links or stable reference IDs, what each shows and why
  it matters here. Separate observations from your inferences.
- Chosen approach and a concrete reason; record alternatives only when useful.
- Missing evidence or tools that materially limit the decision.

If a required source is unavailable, report the limitation before dependent work;
do not silently replace it or claim the instruction was satisfied. Use a fallback
only when consistent with the user's constraints. Where external research is
optional and unavailable, say so and ground a bounded choice in the existing UI
and established patterns. Never invent sources or claim a reference
was inspected. Reading a skill or writing the brief does not authorize edits.
Use existing approved decisions where they already settle the question.

## Build and inspect the result

Implement within the existing coding assignment and host/mode permissions. Use
the project's components and relevant frontend-design guidance when available.
Research downloads, scripts and dependencies belong only in permitted research
locations; do not change app packages just to collect references.

Review the real running page at a representative desktop and phone width, using
available browser tools or Playwright and screenshots. Exercise the affected
flow and relevant loading, empty, error and keyboard/focus states. Inspect
hierarchy, readable text, overflow, spacing, interaction feedback and touch targets.
Prefer existing previews; manage only task-owned processes and retain requested
previews. Do not submit real purchases, messages or production-data changes as
part of visual inspection.

Report concrete findings with viewport/route and the observed effect. Fix defects
within the agreed scope, then recheck affected states. Finish when the task's
acceptance criteria are met; unresolved defects or unavailable browser access
remain explicit. A code review or a mockup is not evidence of a real-page check.
Do not turn a narrow edit into an unbounded polish loop.

## When Fabex is present

Feed the brief and relevant evidence into Fabex's existing independent views and
reconciliation. Respect the coding, documentation and image-review assignments;
a partner without image-review authority uses the assigned reviewer's findings.
If evidence requires another look, request that look through the existing cycle.
Do not duplicate seals, partner cycles or approvals. With one AI and no Fabex,
perform the same research/build/review workflow directly under host permissions.
Modes supplies activity permissions when installed; this skill grants none.
