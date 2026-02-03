# No Man's Sky Notes Project

This directory contains my game notes and reference material for No Man's Sky.

## Workflow Rules

1. **GameMemory.md is the source of truth** - All notes, tips, base info, recipes go here
2. **Git commit on every change** - Each modification to GameMemory.md gets a commit with a descriptive message
3. **Commit message format**: Short summary of the note/memory added (e.g., "Add recipe for X", "New base: Y", "Update base resources")

## Audio Input

Use macOS dictation for hands-free input while playing:
- Press `Command` key twice to start dictation
- Speak your note
- Text appears in terminal, process with Claude

## Note Commands

When I provide input (typed or dictated), for example, I'd use expressions like:
- "Add note: <content>" → Append to relevant section in GameMemory.md, commit
- "New base: <name>" → Add new base section with template, commit
- "Recipe: <item>" → Add to Recipes section, commit
- "Tip: <content>" → Add to General notes section, commit
- "Remember about my base <BaseInfo> that <content>" → Add to Base Info section, commit
- "Add a receipe for <item> for ingredients <content>" → Add to Recipes section, commit
- "Undo the last change". Where change might be commit, update, notes, comment... git revert the last commit.
- "Remember <content>" → determine the relevant section and add to it, or create a new section (asking the user if the section sounds reasonable), commit

## File Structure

- `CLAUDE.md` - This file, project instructions
- `GameMemory.md` - All game notes, bases, recipes, tips

## Git Workflow

After any change to GameMemory.md:
1. Stage the file
2. Commit with message summarizing the addition/change
3. Keep commits atomic (one note/change per commit) for easy revert
