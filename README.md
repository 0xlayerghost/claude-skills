# Claude Skills

A collection of reusable AI agent skills for blockchain developers.

## Skills Included

| Skill | Description |
|-------|-------------|
| [interview](skills/interview/SKILL.md) | Analyze project code, extract technical highlights, and generate interview talking points for blockchain developers. |

---

## Install

### Quick Install

```bash
# Interactive — choose which skills to install
npx skills add 0xlayerghost/claude-skills

# Install all skills at once (no prompts)
npx skills add 0xlayerghost/claude-skills -y
```

### Install for a Specific Agent

```bash
# Claude Code
npx skills add 0xlayerghost/claude-skills -y --agent claude-code

# Cursor
npx skills add 0xlayerghost/claude-skills -y --agent cursor

# Windsurf
npx skills add 0xlayerghost/claude-skills -y --agent windsurf
```

### Install a Single Skill

```bash
npx skills add 0xlayerghost/claude-skills --skill interview
```

## After Install

Copy the `CLAUDE.md` template to your project root so skills are auto-invoked — no `/slash-commands` needed:

```bash
curl -sL https://raw.githubusercontent.com/0xlayerghost/claude-skills/main/CLAUDE.md.template -o CLAUDE.md
```

Or manually copy `CLAUDE.md.template` → `CLAUDE.md` in your project root.

> `CLAUDE.md` is loaded at the start of every Claude Code session. It tells your agent **when** to invoke each skill automatically.

Add to `.gitignore` to keep your repo clean:

```
.agents/
.claude/
.cursor/
.windsurf/
```

## Supported Agents

- [Claude Code](https://claude.ai/code)
- [Cursor](https://cursor.sh)
- [Windsurf](https://windsurf.ai)

## License

MIT
