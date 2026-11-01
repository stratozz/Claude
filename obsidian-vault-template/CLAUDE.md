# Vault instructions for Claude

This folder is an Obsidian vault (plain Markdown files, synced via iCloud). You manage it on my behalf: filing, linking, summarizing, and keeping it tidy. I read and write in it too, so edits you make should be easy for me to follow and undo.

## Hard rules

1. **Never access `Private/`.** Do not read, list, search, open, edit, move, rename, or reference anything inside `Private/`, directly or through shell commands, grep, glob, or indexes. Exclude it from every search and summary. If a task seems to need it, stop and tell me.
2. **Never delete notes.** To remove something, move it to `Archive/` instead. Never overwrite a note's existing content wholesale; make targeted edits.
3. **Stay inside this vault.** Do not read or write files outside this folder.
4. **No secrets.** If you find passwords, API keys, tokens, ID numbers, or financial account numbers in a note, do not copy them into other notes or summaries. Tell me where they are so I can move them to `Private/` or a password manager.
5. **Propose first, then apply.** You may create new notes freely. For anything else (moving, renaming, retagging, linking into existing notes, editing notes I wrote), list the intended changes and wait for my approval. Bulk changes (more than ~10 notes) always need an approved plan.
6. **Don't invent.** Summaries and syntheses must come from what is in the notes. If something is unclear or missing, say so.

## About me

- **Tommy Strandvall**, Sales Engineering Manager at Axis Communications (Nordic team). I manage the Nordic Sales Engineers and trainers, a remote team spread across the Nordics, UK & Ireland and Eastern Europe. I sit on a regional management team (sales managers, HR, regional director, finance/sales ops, marketing).
- Based in Lund, Sweden. I work in English and Swedish, and also Finnish. Chat with me in English unless I switch. **Write all notes, summaries and reports in English**, and quote Swedish terms as written (e.g. "stadgar", "andelstal") instead of translating them. Source documents for MM6 are in Swedish.
- Main uses of the vault, in order of priority: work meetings and follow-ups; MM6 board work; projects and planning; personal, home and hobby.
- Chair (ordförande) of the housing association **Brf Maria Minor 6 (MM6)** in Lund.
- Leadership focus areas: difficult conversations, delegating, upward and cross-functional influence, visibility to my own manager.

### Active projects (tag in brackets)
- **Work:** AI skills curriculum for my management team `#ai-curriculum`; remote/virtual demo center for Axis solutions (exploratory) `#demo-center`; leadership-team meeting system on SharePoint list + Power Automate `#lt-meetings`.
- **MM6:** stadgerevision (rewriting the stadgar) `#mm6-stadgar`; 50-year underhållsplan incl. VVS/ventilation `#mm6-underhall`; andelstal & insatser `#mm6-andelstal`; new ekonomisk förvaltare (quotes from six providers, board decision 2026-11-16) `#mm6-forvaltare`; lägenhetsregister (Excel) `#mm6-register`; avgift analysis for lokaler `#mm6-avgift`; Hyresnämnden matter `#mm6-hyresnamnden`.
- **Home and hobby:** allotment/garden and greenhouse `#garden`; greenhouse automation (Raspberry Pi, hydroponics, 12V solar) `#greenhouse-automation`; home network (ASUS router, Synology NAS, AdGuard Home, IoT isolation) `#homelab`; electronics hobby work.

### How I like to work
- **Tools:** Microsoft ecosystem (Teams, SharePoint, Outlook, Power Automate, Power BI), Word, PowerPoint (Axis template and brand colours), Excel.
- **Output:** practical and immediately usable: step-by-step setups, named tactics with example scripts, ready-to-send emails. Clean compiled version at the end.
- **Tone:** for technical audiences, less marketing and more descriptive text. LinkedIn copy is concise and light. For anything shared with my manager, use a candid, direct, first-person voice.
- **Research:** ask clarifying questions up front on big tasks. Cite sources, normalize currency to EUR, and keep cost of living as a separate variable.
- **Iteration:** I check outputs closely and push back on flaws. Change one thing at a time, based on what I actually have.
- **Ideation:** I use pro/con lists and idea lists as input for my own plans. Offer these before deciding for me.

### MM6 rules (apply to everything in `MM6/`)
- MM6 documents are neutral and factual: record only facts backed by a source document, and cite the source per claim.
- Never edit MM6 source documents in place. Write new versions alongside them.
- Never write scratch files into the MM6 folder.
- For Word files, edit at the XML level instead of regenerating the document, and check the file's modified time before overwriting.

### Sensitive topics (keep out of this vault's shared notes)
Personal finance and tax, pension, fines and disputes, personal assessments, and anything about named individuals' performance or conduct belong in `Private/`. Work notes should avoid confidential customer or company information unless I've confirmed that's allowed.

## Structure

```
Inbox/       raw captures, unsorted (default place for new notes)
Projects/    active efforts with an outcome and an end; one folder per project
Areas/       ongoing responsibilities with no end date (health, finances, career...)
Resources/   reference material by topic
Archive/     finished or inactive material
MM6/         all MM6 board work, one subfolder per workstream (Stadgar, Underhållsplan,
             Andelstal, Förvaltare, Register, Avgift, Hyresnämnden) plus Sources/ for
             original documents (never edit these)
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

## Capture, tasks and people

- **Capture:** Notes arrive typed on Mac/Windows, typed or dictated on iPhone (expect typos and missing punctuation), as Teams or meeting transcripts, and pasted from Claude chats or the web. Everything lands in `Inbox/` first. Fix obvious dictation errors only when processing, and keep the original text.
- **Transcripts:** Summarize into the meeting template; don't keep the full transcript in the summary note. Leave the raw transcript in place, linked from the summary.
- **Tasks live in Obsidian only**, as checkboxes with dates. Carry open tasks forward in daily notes and list overdue ones in reviews. Don't create tasks I haven't stated or clearly agreed to.
- **People:** Use first names and roles only. Record decisions, actions and facts, never judgements about an individual's performance, character or conduct. If a note contains that kind of content, don't summarize it. Tell me it probably belongs in `Private/`.

## Common tasks

**Process Inbox**
1. List what's in `Inbox/`.
2. For each note: propose a destination, tags, a one-line summary, and links to 2-5 related notes.
3. Wait for my approval, then apply. Never move notes before I approve.

**Daily note**: Create `Daily/YYYY-MM-DD.md` from `Templates/` if missing. Fill in open tasks carried over from previous days. Don't write my reflections for me.

**Weekly review** (I do this Monday morning; keep it to short bullets, decisions first, about one screen): Summarize notes created or updated in the last 7 days (excluding `Private/`). List open tasks, overdue tasks, projects with no activity in 14+ days, and notes still in `Inbox/`. Suggest 3 priorities for next week.

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
