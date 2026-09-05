---
name: skills-for-astra
description: Audit and slim agent skills and always-loaded instruction files using progressive disclosure, narrow triggers, and explicit decision boundaries.
metadata:
  short-description: Reduce agent instruction bloat safely
---

# Skills for Astra

Use when a user asks to audit, simplify, or modernize an agent's skills,
`AGENTS.md`, or `CLAUDE.md` without removing useful specialist capability.

## Workflow

1. Inventory active instruction sources separately from plugin caches, templates,
   and inactive/on-demand skills.
2. Measure the real discovery surface: skill descriptions, recursively exposed
   manifests, duplicated names, and always-loaded policy text.
3. Keep descriptions to one discriminating sentence. Move conditional detail to
   `references/`, runbooks, or specialist skills.
4. Preserve specialist workflows as on-demand capabilities; do not delete a
   skill merely because it shares keywords with another.
5. Put durable, cross-task boundaries in global policy. Keep tool manuals,
   credentials, account details, campaigns, and model-specific recipes out of it.
6. Apply only requested changes through the canonical source of truth, then
   verify the resolved runtime surface and configuration integrity.

Read [the audit checklist](references/audit-checklist.md) for a full pass.

## Boundaries

- Treat public publication, deployment, payments, account changes, and agent
  launches as separate actions that require explicit scope in the current task.
- Do not change unrelated agents, campaigns, or consumer runtimes during an
  instruction cleanup.
- Do not claim affiliation with, compatibility with, or endorsement by a model
  provider. The “astra” label is a package name, not a capability guarantee.
