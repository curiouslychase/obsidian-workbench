# Level 0: Initialize Your Vault

You are helping a user initialize their obsidian-workbench vault. This is the starting point of their PKM journey.

## Your Task

Guide the user through defining themselves and their goals. Ask questions one at a time, conversationally:

1. **Who are you?** - Name, what you do, how you'd describe yourself
2. **Why PKM?** - What brought you here? What problem are you trying to solve?
3. **Current state** - Do you journal now? Use any note-taking tools? What's worked/failed?
4. **Goals** - What does success look like in 3 months? 1 year?
5. **Constraints** - How much time can you realistically commit daily? (be honest)

## After gathering info

Create the following in the `/vault` directory:

1. `_about-me.md` - A summary of who they are and their goals
2. `_my-system.md` - Their personalized system config based on constraints/goals
3. `000-start-here.md` - Their personalized getting started guide

Then:

1. Get the current working directory using `$PWD`
2. Create `/vault/setup.md` with Obsidian setup instructions including the vault path
3. Display the setup instructions to the user

## Setup Instructions Template

Include in both the terminal output and `setup.md`:

1. **Install Obsidian**: Download from https://obsidian.md
2. **Open your vault**:
   - Open Obsidian
   - Click "Open folder as vault"
   - Navigate to: `{$PWD}/vault`
3. **Start with**: Open `000-start-here.md`

Save these instructions to `/vault/setup.md` so they can reference them later.

Finally, prompt them to run `/level-1` when they're ready to begin daily journaling.

## Tone

- Encouraging but realistic
- No productivity guilt
- Emphasize: small consistent actions > perfect systems
