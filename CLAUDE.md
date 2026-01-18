# CLAUDE.md

## Project Overview

Think of this as a crawler-type RPG. Users start at Level 0, define themselves and their goals, then progressively unlock new capabilities through consistent practice.

obsidian-workbench is an iterative Obsidian vault builder. Users clone and progressively build their own PKM (personal knowledge management) system through guided weekly levels.

Core principle: Systems are earned through consistent small actions, not downloaded as templates.

## Structure

- `/.claude/commands/` - Claude Code slash commands
- `/vault/` - Working Obsidian vault (all non-Claude content lives here)

## Levels

1. Daily capture (journaling habit)
2. Weekly review (reflection)
3. Linking (connect ideas)
4. Projects (goal organization)
5. Advanced workflows (customization)

## Claude Code Commands

Users progress via slash commands. Each level can have multiple lessons:

```
level-{level}-{lesson}-{action}
```

Examples:
- `level-1-000-setup` - Set up interstitial journaling
- `level-1-001-first-journal-entry` - Create first entry
- `level-2-000-setup` - Configure weekly review

Commands live in `.claude/commands/`. Each level checks prerequisites from previous levels.

## File Naming

**Vault files:**
- Do NOT kebab-case
- Use Title Case with spaces (e.g., `000 OS/`, `My Notes.md`)
- Prefix with `!` to pin files to top (e.g., `!Start Here.md`)

**Command files (.claude/commands/):**
- Use kebab-case (e.g., `level-1-000-setup.md`)

## Philosophy

- Start with one thing, build consistency first
- Earn complexity as habits solidify
- Compound small daily actions into long-term value
