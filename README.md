# inventor-mindset

Makes the agent think like an inventor / research engineer when building something new: first principles, going past the obvious solution, and novel design.

The skill itself is `SKILL.md` plus the `references/` folder. Keep the folder together and named `inventor-mindset`.

## Install

Clone once, then copy (or symlink) into the skills directory of your tool.

```bash
git clone https://github.com/anaslari23/inventor-mindset.git
```

| Tool | Global (all projects) | Project only |
|------|----------------------|--------------|
| Claude Code | `~/.claude/skills/inventor-mindset/` | `.claude/skills/inventor-mindset/` |
| Codex CLI | `~/.codex/skills/inventor-mindset/` | `.codex/skills/inventor-mindset/` |
| Cursor | `~/.cursor/skills/inventor-mindset/` | `.cursor/skills/inventor-mindset/` |
| Antigravity | `~/.gemini/antigravity/skills/inventor-mindset/` | `.agent/skills/inventor-mindset/` |

### Claude Code
```bash
mkdir -p ~/.claude/skills && cp -R inventor-mindset ~/.claude/skills/
```

### Codex
```bash
mkdir -p ~/.codex/skills && cp -R inventor-mindset ~/.codex/skills/
```

### Cursor
```bash
mkdir -p ~/.cursor/skills && cp -R inventor-mindset ~/.cursor/skills/
```
On older Cursor versions without Agent Skills, paste `SKILL.md` into a rule at `.cursor/rules/inventor-mindset.mdc`.

### Antigravity
```bash
mkdir -p ~/.gemini/antigravity/skills && cp -R inventor-mindset ~/.gemini/antigravity/skills/
```
For one workspace only, copy to `<project>/.agent/skills/` instead.

### Claude.ai / Claude Desktop
Zip the `inventor-mindset` folder and upload it under Settings → Capabilities → Skills.

Restart the tool (or start a new session) after installing. Skill paths vary between tool versions; if yours differs, check its skills documentation.

## Usage

Skills load automatically when your request matches the `description` in the `SKILL.md` frontmatter. You can also ask for it by name (`inventor-mindset`).
