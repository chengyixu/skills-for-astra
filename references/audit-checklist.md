# Instruction-surface audit checklist

## Establish the source of truth

- Identify the file or database record that generates each effective global
  policy. Do not patch generated output if it will be overwritten.
- Enumerate active skills, on-demand skills, system-provided skills, and
  plugin/cache/template files independently.
- Inspect consumer roots as well as the registry: a top-level limit can be
  defeated by recursively visible children.

## Review skills

For each active skill, check that its discovery description answers only:
what it does, and when it is the narrowest useful choice.

Flag and repair:

- catch-all or “always use” triggers;
- duplicated declared names or conflicting destinations;
- a router whose children are recursively advertised;
- a root `SKILL.md` that contains a complete manual rather than a routing
  decision;
- stale paths, credentials, or environment claims.

Keep the original detailed procedure in a linked guide or runbook when it is
still useful. A smaller entrypoint should retain real safety constraints, not
silently weaken them.

## Review global instructions

A global policy should contain only stable cross-task rules, such as scope,
verification, language, and explicit-action boundaries. Remove capability
inventories, command cheat sheets, account metadata, recurring campaign
instructions, and unconditional worker counts.

Use contextual skills for browser, desktop, cloud, office, marketing, and
other domain-specific procedures.

## Verify

- Parse changed frontmatter and validate required `name` and `description`.
- Confirm active names are unique and the actual consumer-visible manifest
  count fits its budget.
- Run the registry topology/configuration audit and relevant tests.
- Verify that generated policy files match their canonical source.
- Record what changed, what was intentionally left on-demand, and any public
  claim that requires a separate readback.
