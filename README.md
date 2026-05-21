# seedex-skills

Claude Code skills published by [@wishworldbetter](https://github.com/wishworldbetter).

## Skills

### `spark` — Standalone brainstorming → spec

Turns a vague idea into a written spec document, then stops. No auto-chaining to implementation planning, no surprise next steps. You get the spec; you decide what to do with it.

**Install:**

```bash
npx skills add wishworldbetter/seedex-skills --skill spark
```

This drops the skill into `~/.claude/skills/spark/`. To uninstall:

```bash
rm -rf ~/.claude/skills/spark
```

**What it does:**

- Asks one question at a time to clarify your idea
- Proposes 2–3 approaches with tradeoffs and a recommendation
- Presents the design in sections for your approval
- Writes the final spec to `docs/spark/YYYY-MM-DD-<topic>-design.md` and commits it
- **Stops there.** Hands the spec path back and ends the turn

**When to use:**

When you want to explore an idea before writing any code, and want a written spec out the other end without the assistant immediately running off to implement it.

## Credits

The `spark` skill is extracted from [obra/superpowers](https://github.com/obra/superpowers) (MIT licensed) and modified to:

- Stop after delivering the spec — no auto-chaining to `writing-plans` or any other skill
- Remove cross-skill dependencies that don't exist outside the full Superpowers plugin
- Rename to `spark` to avoid confusion with the original `brainstorming` skill

Original author: Jesse Vincent ([@obra](https://github.com/obra)). The Superpowers methodology this skill comes from is documented in his [original release announcement](https://blog.fsck.com/2025/10/09/superpowers/).

## License

MIT — see [LICENSE](./LICENSE).
