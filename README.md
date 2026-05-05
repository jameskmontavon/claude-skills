# claude-skills

Public Claude Code skills I've built and am happy to share. Use any of them, fork, modify, contribute back if useful.

## What's a Claude Code skill?

A skill is a reusable prompt + workflow that Claude Code can invoke on demand. It's just a markdown file (`SKILL.md`) with frontmatter describing when to use it. When triggered, Claude follows the instructions inside.

Docs: https://docs.claude.com/en/docs/agents-and-tools/agent-skills

## How to use a skill from this repo

Pick a skill below, then copy its directory into your local Claude skills folder:

**Global (skill works in any directory):**
```bash
mkdir -p ~/.claude/skills
cp -R skills/<skill-name> ~/.claude/skills/
```

**Project-specific (skill works only when Claude runs in that project):**
```bash
mkdir -p /path/to/your/project/.claude/skills
cp -R skills/<skill-name> /path/to/your/project/.claude/skills/
```

Restart any active Claude Code session after copying. The skill becomes available as `/<skill-name>` (or auto-invokes per its description).

## Skills

### [`mom-test-questions`](skills/mom-test-questions)

Apply Rob Fitzpatrick's *Mom Test* principles to sharpen meeting questions. Filters out fluff (generic claims, hypothetical maybes, future promises) and rewrites questions to anchor on real past behavior. Useful for interviews, scouting/recruiting calls, reference checks, user research, sales discovery — any conversation where you need true signal rather than polite agreement.

## About me

James Montavon — Biosecurity Specialist at [BlueDot Impact](https://bluedot.org). Most of my Claude Code use is for talent pipeline work, meeting prep, and writing assistance. Skills here will reflect that.

## License

MIT — see `LICENSE`. Use freely.
