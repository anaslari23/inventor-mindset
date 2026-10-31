# inventor-mindset

> Get past the average answer: think like a research engineer, then prove it.

An agent skill for open-ended "build something new" work, where the first plausible solution is usually the generic one.

## What it does

Runs a 7-phase loop and makes the agent show its work:

1. **Reframe** the problem and write measurable success criteria
2. **First principles**: what must be true, and which conventions are only habit
3. **Diverge**: at least three genuinely different approaches (invert, borrow, collapse, extreme, naive-first)
4. **Choose by experiment**: test each candidate's riskiest assumption cheaply
5. **Build the thinnest prototype** and actually run it
6. **Attack your own work** before presenting it
7. **Push once more**: what would make it 10x, not 10%, better?

Output is a short write-up: the idea, why it differs from the obvious approach, evidence, rejected alternatives, known limits, next experiment.

## When it triggers

Designing or prototyping a novel system, algorithm, library, product or AI feature; "think harder", "first principles", "go deeper"; or when you say the first answer isn't good enough. Skipped for trivial edits, lookups and routine CRUD.

## Example prompts

- "Design a cache invalidation scheme for our edge workers. Think from first principles."
- "The obvious approach feels generic. Invent something better for deduplicating these logs."

## Files

- `SKILL.md`: the loop, presentation format and calibration rules.
- `references/thinking-tools.md`: TRIZ, pre-mortem, inversion and other prompts for when you're stuck.

## Install

```bash
git clone https://github.com/anaslari23/inventor-mindset.git
```

Copy the `inventor-mindset` folder into your tool's skills directory, then restart it or open a new session.

| Tool | Global (all projects) | Project only |
|------|----------------------|--------------|
| Claude Code | `~/.claude/skills/inventor-mindset/` | `.claude/skills/inventor-mindset/` |
| Codex CLI | `~/.codex/skills/inventor-mindset/` | `.codex/skills/inventor-mindset/` |
| Cursor | `~/.cursor/skills/inventor-mindset/` | `.cursor/skills/inventor-mindset/` |
| Antigravity | `~/.gemini/antigravity/skills/inventor-mindset/` | `.agent/skills/inventor-mindset/` |

One-liner (Claude Code, global):

```bash
git clone https://github.com/anaslari23/inventor-mindset.git ~/.claude/skills/inventor-mindset
```

- **Cursor without Agent Skills:** paste `SKILL.md` into `.cursor/rules/inventor-mindset.mdc`.
- **Claude.ai / Desktop:** zip the `inventor-mindset` folder and upload it under Settings → Capabilities → Skills.
- Paths vary by tool version; check your tool's skills docs if one doesn't load.
- To update later: `git -C <install path> pull`.

## License

MIT, see [LICENSE](LICENSE).
