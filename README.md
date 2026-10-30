# skills

A collection of modular, self-contained AI agent skills. Each skill is a single folder with a `SKILL.md` file.

## Installation

Pick one route. Installing both creates duplicate skills.

### Option 1: skills.sh (editable files)

Interactive picker:

```bash
npx skills@latest add pererikbergman/skills
```

Specific skill:

```bash
npx skills@latest add pererikbergman/skills/<skill-name>
```

### Option 2: Claude Code plugin (read-only bundle)

From the GitHub marketplace manifest:

```bash
claude plugin marketplace add pererikbergman/skills && claude plugin install skills@pererikbergman
```

From the official Claude plugins directory:

```bash
claude plugin install skills@claude-plugins-official
```

## Repository Structure

```
.
├── .claude-plugin/
│   ├── marketplace.json
│   └── plugin.json
└── skills/
    └── <skill-name>/
        └── SKILL.md
```

## Skill Format

Each `SKILL.md` starts with YAML frontmatter, followed by Markdown instructions:

```markdown
---
name: <skill-name>
description: <when to use this skill>
---

# <Skill title>

<Instructions in Markdown>
```

## Skill Index

| Skill | Description |
| ----- | ----------- |
