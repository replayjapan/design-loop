# Design Loop

## FOR HUMANS

Design Loop helps your AI research a UI decision before building, then inspect
what actually shipped in the browser. It keeps research proportionate: a small
layout correction needs a small check, not a redesign exercise.

Install this standalone Claude Code plugin from its marketplace:

```text
/plugin marketplace add https://github.com/replayjapan/design-loop.git
/plugin install design-loop@design-loop
```

If you already use the Fabex marketplace, update it and install from there instead:

```text
/plugin marketplace update fabex
/plugin install design-loop@fabex
```

Reload plugins, then ask for a UI change or use `/design-loop:design-loop` with
your task. The AI produces a short brief connecting relevant sources to design
choices, builds within your existing authorization, and reviews the real page
at desktop and phone widths. You get concrete findings and any remaining limits.
Research tools and a browser are not bundled. Missing tools are reported; the
plugin does not install them or pretend to have inspected a page.

If you specify a research source, Design Loop keeps using it for relevant UI
decisions until you change that instruction. Each new UI request returns to
research before building. It also checks whether proposed elements help the task
and preserve spacing and hierarchy, raising conflicts before crowding the page.

Design Loop works with one AI. With Fabex, it contributes to the existing partner
review and follows its image-review assignment. It adds no hooks, background
processes or extra review cycle. Modes and AI Usage Tracker are optional,
independent plugins. Installing Design Loop does not change their settings.
With Modes installed, use `/modes:discussion` for research and planning and
`/modes:work` for authorized implementation. With Fabex alone, the host's plan
mode controls discussion; `/fabex:settings` controls task assignments and
`/fabex:session` controls conversations. Design Loop itself has no activity or
conversation settings. Your own design guidelines always take priority over the
references it finds.

Examples:

- “Improve this settings page without changing its navigation.”
- “Research a mobile checkout pattern, then implement the agreed flow.”
- “Review the running page for desktop and phone layout problems.”

### Related plugins

These plugins work together, and each one also works on its own.

| Plugin | What it does |
| --- | --- |
| [Fabex](https://github.com/replayjapan/fabex) | Claude and Codex work as partners: each considers your request independently, then they agree before acting. |
| [Modes](https://github.com/replayjapan/modes) | Choose what your AI may do right now: build, research and plan, or just answer a question. |
| [AI Usage Tracker](https://github.com/replayjapan/ai-usage-tracker) | See your remaining Claude and Codex allowance and where a project's tokens went. |
| [Publish Guard](https://github.com/replayjapan/publish-guard) | Reviews supported Git and GitHub actions for private information before they are published. |

## FOR AI BROTHREN

Use [the Design Loop skill](skills/design-loop/SKILL.md) for meaningful UI work.
Preserve the user's product, constraints and authorization. Inspect existing UI
before choosing references. A brief is evidence for a decision, not approval to
build. Research and browser interactions stay within host and mode permissions.

Without Fabex, one AI performs the workflow. With Fabex, both partners receive
relevant findings before their existing reconciliation; only the assigned coder
edits, and the assigned image reviewer inspects screenshots. Do not create a
second independence/sealing cycle or spawn helpers without authorization.

This repository contains skill instructions and Claude plugin/marketplace
metadata only. It has no runtime dependencies or hooks. Validate the JSON,
skill frontmatter and relative links, then review the skill against a small UI
change, unavailable research/browser tools and a Fabex-assigned image reviewer.
Never report browser checks as completed when only source code was inspected.

MIT license. Copyright rePlay, LLC.
