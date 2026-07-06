# spark

Standalone brainstorming skill. Asks one question at a time to refine an idea, presents 2-3 approaches with tradeoffs, writes a spec to `docs/spark/YYYY-MM-DD-<topic>-design.md`, then stops.

See [SKILL.md](./SKILL.md) for the full skill content.

## Provenance

Extracted from [`brainstorming`](https://github.com/obra/superpowers/tree/v6.0.0/skills/brainstorming) in [obra/superpowers](https://github.com/obra/superpowers) v6.0.0 (MIT, Jesse Vincent).

This fork keeps the Superpowers 6.0 brainstorming updates, including the just-in-time visual companion flow and the updated authenticated/restartable companion server.

## Spark Changes

Functional intent: upstream `brainstorming` ends by handing off to `writing-plans`, which then continues into implementation planning. `spark` cuts the pipeline at the spec. Once the spec is written and reviewed, the skill reports the spec path and stops.

Local changes from upstream:

- Frontmatter is renamed from `brainstorming` to `spark`, with `version: 0.2.0`.
- Spec output path is `docs/spark/YYYY-MM-DD-<topic>-design.md`.
- The terminal state is `Deliver spec path to user and STOP`, not `Invoke writing-plans skill`.
- The optional `elements-of-style` cross-skill dependency is removed.
- The visual companion reference points to this skill directory's `visual-companion.md`.

## Preserved From Superpowers 6.0

- 9-step brainstorming checklist and hard gate before implementation.
- Just-in-time visual companion offer: only when a question is clearer shown than described.
- Authenticated visual companion URL with session key, restart support, and project-local `.superpowers/brainstorm/` state.
- Spec self-review loop for placeholders, contradictions, scope, and ambiguity.
- The `spec-document-reviewer-prompt.md` reviewer template.

## License

MIT - see [LICENSE](../../LICENSE) at the repository root.
