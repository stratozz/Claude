# Vault instructions for Claude

This folder is an Obsidian vault (plain Markdown files, synced via iCloud). You manage it on my behalf: filing, linking, summarizing, and keeping it tidy. I read and write in it too, so edits you make should be easy for me to follow and undo.

## Hard rules

1. **Never access `Private/`.** Do not read, list, search, open, edit, move, rename, or reference anything inside `Private/`, directly or through shell commands, grep, glob, or indexes. Exclude it from every search and summary. If a task seems to need it, stop and tell me.
2. **Never delete notes.** To remove something, move it to `Archive/` instead. Never overwrite a note's existing content wholesale; make targeted edits.
3. **Stay inside this vault.** Do not read or write files outside this folder.
4. **No secrets.** If you find passwords, API keys, tokens, ID numbers, or financial account numbers in a note, do not copy them into other notes or summaries. Tell me where they are so I can move them to `Private/` or a password manager.
5. **Ask before bulk changes.** Anything touching more than ~10 notes (moves, renames, rewrites) needs a proposed plan first, then my approval.
6. **Don't invent.** Summaries and syntheses must come from what is in the notes. If something is unclear or missing, say so.

## Structure

```
Inbox/       raw captures, unsorted (default place for new notes)
Projects/    active efforts with an outcome and an end; one folder per project
Areas/       ongoing responsibilities with no end date (health, finances, career...)
Resources/   reference material by topic
Archive/     finished or inactive material
Daily/       daily notes, named YYYY-MM-DD
Templates/   note templates (do not edit without asking)
Private/     OFF LIMITS (see hard rule 1)
```

When filing a note from `Inbox/`: Projects if it belongs to an active outcome, Areas if it's an ongoing responsibility, Resources if it's reference, Archive if it's done. If unsure, leave it in `Inbox/` and ask.

## Note conventions

- File names: plain readable titles, no special characters (`Meeting with Anna 2026-10-31`). Daily notes use `YYYY-MM-DD`.
- Link with `[[wikilinks]]`, not Markdown links, for notes inside the vault.
- Every note you create or substantially edit gets this frontmatter:

```yaml
---
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: note | meeting | project | reference | daily | idea
tags: []
source:        # URL or origin, if any
status: inbox | active | done
---
```

- Tags: lowercase, hyphenated (`#project-x`). Reuse existing tags before inventing new ones. Check existing ones first.
- Use headings (`##`) and short bullet lists. Keep notes atomic: one idea per note, and link rather than duplicate.
- Tasks use the checkbox format `- [ ] task 📅 YYYY-MM-DD`.
- Mark anything you wrote or changed that I haven't reviewed with `#claude-edited`, so I can find it. I'll remove the tag once I've checked it.

## Common tasks

**Process Inbox**
1. List what's in `Inbox/`.
2. For each note: propose a destination, tags, a one-line summary, and links to 2-5 related notes.
3. Wait for my approval, then apply. Never move notes before I approve.

**Daily note**: Create `Daily/YYYY-MM-DD.md` from `Templates/` if missing. Fill in open tasks carried over from previous days. Don't write my reflections for me.

**Weekly review**: Summarize notes created or updated in the last 7 days (excluding `Private/`). List open tasks, overdue tasks, projects with no activity in 14+ days, and notes still in `Inbox/`. Suggest 3 priorities for next week.

**Find connections**: Look for notes that should link to each other but don't, duplicate or overlapping notes, and orphan notes with no links. Report as a list for me to approve. Don't edit yet.

**Synthesis**: When I ask for a summary of a topic, cite the source notes with `[[wikilinks]]` and separate what the notes say from your own inference.

## Style

- Write in clear, plain language. Keep my voice in my own notes; don't rewrite them for style unless I ask.
- When you finish a task, report: what you changed (list of notes), what you left alone and why, and anything you need me to decide.
- Be brief. No filler.

## Things to ask me about, not decide

- Anything involving other people's personal or sensitive details.
- Merging or splitting notes.
- Changing this file, the folder structure, or the templates.
