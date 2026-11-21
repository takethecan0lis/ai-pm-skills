---
name: session-snapshot
description: Keeps a project's memory outside the conversation, in four living files (work log, decision log, resume note, backlog), so any new session can pick up where the last one stopped. Defines what is appended and what is overwritten, captures decisions the moment they are agreed, and takes a full snapshot at the triggers the person chooses: on request, when they say they are finished, and before the conversation is summarized or reset. The resume note opens with the few decisions the owner must make. Use when work spans several sessions, when a session is about to end or be compacted, or when you start a session and need to know where things stand.
---

# Session snapshot

## Objective and benefit
**Objective:** At any moment, the project's state lives in four short files, so a fresh session can resume work after reading two of them.

**Benefit:** It aims to stop work from depending on what one conversation happens to remember. Decisions are recorded once, in a place that can be searched, and the resume note puts the owner's open questions at the top. Without it, context is often lost between sessions, decisions can be made twice, and the owner may have to retell the story.

**Why it is worth having:** It buys continuity, and the proof is a clear record of what was done and why that anyone can check.

## When to use
- A project runs across more than one session, or across context resets.
- You are about to end a session, or the conversation is about to be summarized or cleared.
- You are starting a session and need to know where things stand.
- Skip it for a one-off question with no follow-up work.

## Personalize it: questions to ask first
Before the first snapshot, ask the person these questions. Each is a personal choice: ask, do not assume. Ask one at a time, in plain words, offer the suggested default, and accept "use the default". Write the answers into a short preferences note (a template is in PREFERENCES-TEMPLATE.md) and read it before every snapshot. If an answer changes, update the note and say so.

First session: ask only questions 1, 2 and 3. The rest use their defaults and are asked again after the first snapshot.

1. Where should the four files live, and what should they be called? (Suggested default: a single folder at the root of the project, with plain descriptive names that match anything already there.)
2. What must never be written to the logs: private projects, names, amounts, anything else? (No default. Ask for kinds of things, for example: client names, money amounts, health, anything about a named person.)
3. What should the resume note open with, and how many asks at most? (Suggested default: the open decisions, a small handful at most.)
4. How often should you snapshot, what should trigger one, and should you ask before taking one when the conversation is about to be shortened? (Suggested default: when the person asks or says they are finished, and before the conversation is shortened or cleared, without asking first, because nothing is lost by it.)
5. How long should old entries stay in the main files, and where do older ones go? (Suggested default: keep recent entries in place and move older ones to an archive file beside them, never deleting.)
6. Only if you use a tool that shortens the conversation: do you want a short closing line asking whether to shorten it now? (Suggested default: no, unless the person wants it.)

If the person cannot answer yet, use the defaults, mark them as defaults in the note, and ask again after the first snapshot. Until question 2 is answered, keep out personal, health and financial details.

## Steps
1. **Find or create the four files.** Look for files that already do these jobs and adopt them rather than making duplicates. Before the first write, tell the person which files you will create or change and where, and wait for a yes. Then create only what is missing, in the style the existing files use.
2. **Know the roles.**
   - Work log: what was done, newest entry first. Append only.
   - Decision log: one entry per decision, each with a stable ID and a status. A changed decision gets a new entry that points to the one it replaces, and the old entry stays, crossed out and pointing to the newer one. Never delete.
   - Resume note: the one file that is overwritten whole each time. It is the first thing read in a new session.
   - Backlog: future work and ideas, with status and priority.
3. **Capture as it happens.** When a decision is agreed or a backlog item is identified, write it down right then. A snapshot reviews and completes what is already there; it is not the first time anything is recorded.
4. **Start of a session.** Read the resume note and the decision log before doing real work. Mention any open blockers to the owner first. Then tell the person in two lines where things stand and which decisions are waiting on them. Do not read the files out.
5. **Before adding a decision,** search the decision log for the topic. If one exists, replace it: add the new entry, cross out the old one and point to the newer one. Do not add a second entry on the same question.
6. **Take a full snapshot** at the triggers in the preferences note; with none set, when the owner asks or says they are finished, and before any summarization or reset of the conversation. Treat 'I'm done', 'thanks, that's all' or a clear closing statement from the person as the end. Save quietly, then say one line: 'Saved. Next time I'll pick up at <focus>.' Do not interrupt work in progress. If a reset happened without a snapshot, take it first, before other work.
7. **Make the first line say what was captured and what was not.** For example, which files were updated and which sources were not reviewed. A partial snapshot calls itself partial.
8. **Append to the work log.** Add a dated entry, newest on top, short and factual: what was done, with counts where you have them.
9. **Update the decision log** with anything agreed since the last snapshot, using the next ID and marking any supersessions.
10. **Overwrite the resume note whole.** Follow the opening and limit in the preferences note. Then current focus and next actions. If nothing needs the owner, say so in one line.
11. **Review the backlog.** Add newly discussed items, and mark finished or dropped ones. Dropped items stay, with the reason.
12. **Keep sensitive material out.** For anything the owner marked private, record counts and links to where it lives, never the content. Leave out names, amounts and details that could identify a person or client when the owner asked for that. Never write passwords, keys or tokens to any log.
13. **Tell the owner what changed** in a few lines, in plain words.

## Example
Invented data. Product team "Pebble Notes", snapshot dated 2026-03-09.

Resume note, top part:

> **Decisions needed**
> 1. Ship offline mode to a 10 percent group first, or to everyone? Recommended: the 10 percent group. Answer:
>
> **Other open questions**
> - Rename the "Teams" tab? Recommended: keep the name (asked 2026-03-07).
>
> **In progress**
> - Export redesign: 4 days, owner Sam, blocked on the file format choice.
>
> Snapshot of 2026-03-09. Captured: all four files. Not captured: the support inbox, which was not reviewed.

Decision log line:

> Decision 14: Offline mode ships to a 10 percent group first (2026-03-09). Replaces decision 11.

Work log line:

> 2026-03-09: Offline mode passed sync tests on phones; tablets not yet tested. Two backlog items added, one closed.

## What this does not verify
- It does not check that what was written is true or complete. A snapshot is only as good as the session's own account.
- It does not stop anyone writing private material into the logs; the owner's list of exclusions has to be followed.
- It does not keep two people or two sessions from editing the same file at once.
- Adopted, not measured: no result is claimed for fewer repeated decisions or faster restarts.

## Common failure modes
- Decisions saved only at snapshot time, so a crash or reset loses them.
- The resume note appended to instead of overwritten, so it grows into a second log.
- Questions buried below the news in the resume note.
- A new decision added beside an older one on the same topic, leaving two answers in the log.
- Deleting replaced entries, so nobody can see why things changed.
- A first line that says "done" without saying what was left out.
- Sensitive content copied into the logs instead of counted and linked.
- A reset or summarization that happens before the snapshot.

CC BY 4.0. Attribution: Drew Podwal. Version 0.1, 2026-11-21. Adopted, not measured: no result has been measured yet.
