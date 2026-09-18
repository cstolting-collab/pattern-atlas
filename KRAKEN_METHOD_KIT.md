# Kraken Method Kit

> **Discovery Mode — 09-18-2026**
>
> A fictional, evidence-bound casefile method for organizing records for personal understanding or attorney review. It is not a finding of fact, a medical opinion, legal advice, or a substitute for counsel.

## Public boundary

This kit intentionally contains no real names, facilities, case numbers, locations, dates tied to a real event, medical facts, documents, or identifying combinations of details. Do not publish material merely because names have been removed: unique dates, places, roles, events, case identifiers, quoted text, and document metadata can still identify people.

Use only records you own, are authorized to use, or that are public. Keep unredacted legal, medical, financial, or personal records in a secure private workspace and obtain legal advice before sharing them externally.

## The purpose

The method answers narrow questions without converting a pattern into an accusation:

1. What is actually documented?
2. When did each documented item occur or become known?
3. Who or what record may answer the next unanswered question?
4. What does the material *not* establish?

## Evidence classes

| Status | What it supports | What it does not support by itself |
|---|---|---|
| `PRIMARY_RECORD` | The content of an original record, within its date and scope | Broader conclusions not stated in the record |
| `FIRSTHAND_ACCOUNT` | What the speaker recalls or reports | Independent verification, intent, diagnosis, or causation |
| `ALLEGATION` | What a complaint or claim alleges | That the allegation is true or liability exists |
| `SECONDARY_LEAD` | A lead worth locating in its original source | A verified fact |
| `HISTORICAL_RECORD` | A prior state at the stated date | The present state |
| `UNKNOWN` | A precise unanswered gap | That the missing record proves failure |

An order supports only what the court actually decided. A docket supports procedural events. A bill supports the provider, date, service description, charge, and claim information shown—not diagnosis, consent, medical necessity, ownership, or liability.

## File structure

```text
00_Counsel_Review.md        # narrow questions and requested decisions
01_Master_Brief.md          # one-page neutral overview
02_Evidence_Map.csv         # workstream: complete / partial / missing
03_Evidence_Records.csv     # source, date, locator, status, limit
04_Timeline.csv             # dated event or observation, linked source ID
05_Relationship_Map.csv     # typed edge, status, effective/observed date
06_Action_Queue.csv         # next record/action, owner, reason, status
07_Document_Index.csv       # document ID, filename, version, hash, locator
08_Corrections_Log.md       # append-only correction history
09_Public_Redaction_Check.md
10_Handoff_Prompt.md
fixtures/                   # fully fictional sample data only
```

Preserve earlier snapshots. Append corrections; do not overwrite history.

## Relationship discipline

Use typed edges, not vague lines: `LICENSEE_OF`, `CONTROLLING_INTEREST_IN`, `ADMINISTRATOR_OF`, `REGISTERED_AGENT_FOR`, `NAMED_IN_COMPLAINT`, `SHARES_ADDRESS_WITH`, or `MENTIONED_IN_RECORD`.

Keep owner, officer, registered agent, manager, administrator, medical professional, management-company role, and allegation defendant separate. A shared address, recurring LLC, officer, lawsuit, or regulatory record does not by itself prove negligence, causation, control, money flow, common enterprise, or bedside authority.

## Workflow

1. **Freeze the question.** State one narrow question that a record can answer.
2. **Index before interpreting.** Assign each source a stable ID, date, type, locator, and evidence class.
3. **Build the dated timeline.** Separate what happened, what was reported, and what is unknown.
4. **Map only documented edges.** Attach a source note and effective/observed date to every relationship.
5. **Separate workstreams.** Keep event chronology, records/billing, regulatory material, ownership/authority, litigation, and comparator research distinct.
6. **Record the limits.** Each entry states what it supports and what it does not establish.
7. **Queue the next record.** Ask for the one source most likely to resolve a specific gap; do not replace missing private records with broad public searching.
8. **Handoff cleanly.** Give counsel the master brief, source index, open questions, and requested records—not a conclusion.

## Fictional example

| ID | Date | Status | Entry | Source / limit |
|---|---:|---|---|---|
| `DOC-001` | 2024 | `PRIMARY_RECORD` | Fictional facility profile lists an operating entity | Supports only the listed role at the displayed date |
| `ACC-001` | 2024 | `FIRSTHAND_ACCOUNT` | Fictional family note reports a missed call | Requires underlying call log to verify occurrence |
| `LEAD-001` | 2025 | `SECONDARY_LEAD` | A news item references a regulatory action | Locate the original order before treating it as fact |
| `Q-001` | — | `UNKNOWN` | Who received a specific notice? | Request the notice log and recipient record |

## Public-release check

Before publishing, remove or replace:

- names, initials, aliases, faces, signatures, account numbers, addresses, phone numbers, emails, and usernames;
- case numbers, claim numbers, facility/provider identifiers, document IDs, and unique locations;
- precise dates, rare event sequences, quotations, metadata, filenames, hidden spreadsheet fields, revision history, and image EXIF data;
- medical, legal, financial, or family information; and
- any combination that could reasonably identify a person or case.

Use fictional examples, not "lightly anonymized" real records. Have a qualified attorney review anything connected to an active matter before publication.

## Honest Application Prompt

```text
You are helping review a fictional or authorized evidence map.

Use only the records and source notes provided. Label each statement as a direct record, firsthand account, allegation, secondary lead, historical record, or unknown. Do not invent missing facts or infer motive, fault, diagnosis, causation, legal liability, guilt, organizational control, or identity from a visual connection.

For each answer: (1) state the narrow question; (2) identify the specific source and locator used; (3) state what the record supports; (4) state what remains unknown; and (5) list the next specific record or question. If the materials do not establish something, say: “The provided materials do not establish this.”
```

## Non-claim statement

This kit organizes information. It does not certify evidence, determine privilege, establish legal or clinical truth, or accuse a person or organization of wrongdoing.
