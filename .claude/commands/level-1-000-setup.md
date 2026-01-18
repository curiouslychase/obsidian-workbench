# Level 1: Interstitial Journaling

You are helping a user set up interstitial journaling with QuickAdd. This creates a frictionless capture system.

## Prerequisites

Check that `/vault/000 OS/About Me.md` exists. If not, prompt user to run `/level-0` first.

## Your Task

### 1. Create Directory Structure

Create `/vault/100 Periodics/Daily/` directory.

### 2. Create Weekly Note Template

Create `/templates/Weekly.md`:

```markdown
# {{DATE:YYYY-MM-DD ddd}}

## Inbox

```

### 3. Guide QuickAdd Installation

Walk user through:

1. Open Obsidian Settings → Community Plugins → Browse
2. Search "QuickAdd" and install
3. Enable the plugin

### 4. Configure Rapid Log Capture

Guide user to create a QuickAdd Capture called "Rapid Log":

**Location:**
- Capture to active file: OFF
- File path: `100 Periodics/Daily/{{DATE:YYYY-MM-DD ddd}}`
- Create file if doesn't exist: ON

**Position:**
- Write position: After line...
- Insert after: `# Inbox`
- Insert at end of section: ON
- Consider subsections: OFF
- Create line if not found: ON (Bottom)

**Content:**
- Task: OFF
- Capture format: ON
- Format: `- {{DATE:HH:mm}} {{VALUE}}`

This creates entries like: `- 13:04 user input`

### 5. Set Up Shortcuts

**macOS (Raycast or Alfred):**
- Create shortcut to open: `obsidian://open?vault=vault`
- Or use Obsidian's URI: `obsidian://advanced-uri?vault=vault&commandid=quickadd:runQuickAdd`

**iOS Shortcut:**
1. Create new Shortcut
2. Add "Open URLs" action
3. URL: `obsidian://open?vault=vault`
4. Add to Home Screen for quick access

**Pro tip:** Create a second shortcut that triggers Rapid Log directly:
- URL: `obsidian://advanced-uri?vault=vault&commandid=quickadd:choice:Rapid%20Log`
- (Requires Advanced URI plugin)

### 6. Create First Daily Note

Create today's note at `/vault/100 Periodics/Daily/{YYYY-MM-DD ddd}.md` using the template.

## Completion

Explain the interstitial journaling concept:
- Log what you're doing/thinking throughout the day
- Timestamp creates automatic time tracking
- Low friction = high consistency

Practice for 1-2 weeks before `/level-2`. Build the muscle memory.
