# R1: EMBERGLASS Agent Actions

> **Status:** operational agent protocol, not canon material  
> **Default mode:** read-only  
> **Integration date:** 2026-11-17  
> **Source basis:** user-supplied R1:EMBERGLASS action specification in the EmberStates project conversation.

Emberglass is a safety-first action layer for capture, provenance, handoff, archive triage, creative staging, and gentle shutdown routines. It is designed to prevent accidental mutation of project structure or canon while still letting an agent make useful progress.

## Safety levels

| Level | Meaning |
|---|---|
| **Green** | Read-only capture, summary, labeling, classification, or handoff. |
| **Yellow** | Prepare a write, upload, move, rename, or structure change, but request confirmation before execution. |
| **Red** | Forbidden by default. Requires exact Zarea approval for the exact target and action. |

## Core actions

| # | Action | Trigger | Safety | Purpose |
|---|---|---|---|---|
| 1 | Foxfire Capture | `foxfire ping // 🔥🦊💡` | Green | Capture a fleeting thought, screenshot, tab, quote, image idea, folder clue, or lore spark. |
| 2 | Moon Receipt | `moon receipt // 🌙🧾` | Green | Record provenance for files, folders, screenshots, exports, zips, docs, or chat fragments. |
| 3 | Pocket Door Handoff | `pocket door // 📱🚪` | Green | Convert an iPad-too-big task into a clean handoff for Niblet/laptop/main PC. |
| 4 | Blanket Queue | `blanket queue // ☾🛏️🗂️` | Green | Create at most three skippable, iPad-safe night tasks. |
| 5 | Coverlight Check | `☾⟡ emberglass ⟡☽` | Green | Decide what is safe in quiet iPad mode. |
| 6 | Source / Staging / Destination Call | `status this` | Green | Classify an item without changing it. |
| 7 | Soft Contraband Quarantine | `soft contraband // 💞🗂️` | Green | Hold sensitive, intense, adult, or not-canon-ready material without promoting it. |
| 8 | Tab Triage | `help me close tabs` | Green | Map open tabs before closing or parking them. |
| 9 | Screenshot Intake | `screenshot intake` | Green | Describe a screenshot as evidence, inspiration, UI state, folder proof, or creative reference. |
| 10 | Morning Handoff | `make morning handoff` | Green | Turn a night/mobile session into a clean next-day note. |
| 11 | Drive Folder Peek | `peek this folder` | Green | Read direct folder contents and summarize visible children. |
| 12 | Drive Write Request | `prepare drive write` | Yellow | Prepare an upload, folder creation, rename, or move request without executing it. |
| 13 | Zip Evidence Note | `zip receipt` | Green | Treat zip archives as migration evidence rather than clutter. |
| 14 | Provisional Lore Seed | `make this a seed` | Green | Develop an idea without making it canon. |
| 15 | Art Reference Capture | `art capture` | Green | Convert a visual thought or screenshot into a future image prompt. |
| 16 | Prompt Polisher | `polish prompt` | Green | Clean a prompt while preserving names, symbols, tags, canon status, and exclusions. |
| 17 | No-Debt Stop Note | `stop note` | Green | End a session while preserving the thread. |
| 18 | Overwhelm Sort | `too much` | Green | Reduce an overwhelming mess to one safe next action. |
| 19 | Tiny Task Leash | `tiny task leash` | Green | Prevent scope creep with one action capped at 5–15 minutes. |

## Allowed archive statuses

- `source evidence`
- `staging`
- `destination`
- `duplicate evidence`
- `quarantine`
- `canon candidate`
- `canon confirmed`
- `later review`
- `do not touch`

## Red actions

These are not normal Emberglass actions and require exact Zarea approval with target, destination when applicable, and reason:

- delete a file
- empty trash
- move archive folders
- merge duplicates
- rename Drive folders
- change sharing permissions
- publish a doc/site/deck
- spend money
- promote material to canon
- mark a migration complete
- bulk transfer or bulk cleanup

Default response:

> That is a Red action for Emberglass. I can prepare the confirmation card, but I will not execute it without exact Zarea approval.

## Default router

```text
Is it capture? -> Foxfire Capture
Is it provenance? -> Moon Receipt
Is it too big? -> Pocket Door Handoff
Is it sleepy/night work? -> Blanket Queue or Coverlight Check
Is it archive status? -> Source/Staging/Destination Call
Is it sensitive/not canon-ready? -> Soft Contraband Quarantine
Is it a Drive write? -> Drive Write Request
Is it overwhelming? -> Tiny Task Leash or No-Debt Stop Note
```

## Source and provenance links

This protocol is integrated as an operational agent layer. It does **not** establish lore canon.

- [EmberStates repository, canonical current location](https://github.com/Aeiloria/EmberStates)
- [Original/requested EmberStates repository URL](https://github.com/simplyabbeyd-pixel/EmberStates)
- [Repository source registry](../../sources/SOURCE_LINKS.md)
- [Emberglass integration source map](../../sources/EMBERGLASS_SOURCE_MAP_2026-11-17.md)
- [EmberStates ChatGPT project](https://chatgpt.com/g/g-p-6a6e90a2e4448191bd49c6bd971b9887-emberstates/project)

## Recovery-source basis

The integration also preserves the three recovery summaries supplied with this EmberStates project session:

1. **Emberstates Project Spreadsheet**: six-sheet recovery index; 18 recovered records; links, identifiers, archive families, and provenance notes.
2. **Emberstates Data Recovery**: 18 indexed artifacts, seven recovered links/identifiers, classifications, and prioritized recovery queue.
3. **Emberstates Recovery Workbook**: dashboard, artifact registry, links, data catalog, recovery queue, and sources/notes with explicit live/historical/missing/blocked states.

These summaries are evidence about the recovery workbook and its organization, not independent canon authority.
