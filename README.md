# Pattern Atlas

> **Discovery Mode — 09-18-2026**
>
> An early public tool for careful, human-led pattern review. It makes no finding or claim beyond the records a person chooses to map.

Pattern Atlas is a local-first browser tool for turning scattered, user-owned records into a source-aware timeline and relationship map.

It answers three bounded questions:

1. What is documented, and when?
2. Which typed relationship connects two visible records?
3. What remains unknown or needs verification?

## What it is not

Pattern Atlas does not infer motive, fault, diagnosis, causation, legal liability, guilt, organizational control, or identity. A visual connection is only a documented relationship with a stated source and date.

It is not a tracker. Use it only for your own records, information you have permission to use, or fully public historical material. Do not use it to identify, profile, or make claims about private people.

## Run locally

Download or clone this repository and open `index.html` in a current browser. There is no server, account, database, API call, analytics, or upload.

## Features in v0.1

- Dated people, organizations, places, documents, and events
- Typed, source-noted relationships
- Year timeline and status/type filters
- “Explain connection” path view
- Local browser storage only
- JSON import/export
- HAP (Honest Application Prompt) builder
- Fictional sample data only

## Data model

Each record needs a name, type, year, and source note. Each relationship needs two records, a typed label, year, evidence status, and source note.

Evidence statuses are:

- Primary / direct record
- Historical record
- Lead needing verification
- Reported allegation

## HAP

HAP creates a bounded prompt to use only in an environment you have approved for the relevant information. It asks an AI to explain provided records without inventing facts or converting patterns into conclusions.

## Project boundary

Pattern Atlas is independent from CML, Repo Darla, Glass House, and any private legal, medical, or personal project. It contains no private data or rules from those projects.

## License

MIT. Copyright 2026 Sherrie Joseph.
