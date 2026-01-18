# CLAUDE.md

## Project Overview

Think of this as a crawler-type RPG. Users start at Level 0, define themselves and their goals, then progressively unlock new capabilities through consistent practice.

obsidian-workbench is an iterative Obsidian vault builder. Users clone and progressively build their own PKM (personal knowledge management) system through guided weekly levels.

Core principle: Systems are earned through consistent small actions, not downloaded as templates.

## Structure

- `/levels` - Progressive guides, one per level
- `/templates` - Obsidian templates that unlock with progress
- `/workflows` - Claude Code workflows for each level
- `/vault` - Working Obsidian vault

## Levels

1. Daily capture (journaling habit)
2. Weekly review (reflection)
3. Linking (connect ideas)
4. Projects (goal organization)
5. Advanced workflows (customization)

## Claude Code Commands

Users progress via slash commands that build on each other:

- `/level-0` - Initialize vault, define goals and constraints
- `/level-1` - Set up daily journaling practice
- `/level-2` - Add weekly review (coming soon)
- `/level-3+` - Progressive unlocks

Commands live in `.claude/commands/`. Each level checks prerequisites from previous levels.

## Philosophy

- Start with one thing, build consistency first
- Earn complexity as habits solidify
- Compound small daily actions into long-term value
