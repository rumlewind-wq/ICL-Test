---
title: Repository Governance
topic: repo governance
type: concept
related: []
tags: ["governance", "automation"]
---

# Repository Governance

Defines metadata standards, automation rules, and Codex workflows for this vault.

## Metadata standard
Add the following YAML block to every note:
```
---
title: <Note title>
topic: <short slug>
type: [case | doctrine | article | concept]
related: []
tags: []
---
```

## Naming conventions
- No prefixes such as “ICL – …”.
- Case notes use `Case <identifier> <Party>.md` (e.g., `Case C-204.08 Rehder v Air Baltic`).
- Singular nouns for doctrine notes (`Arbitral Award`, `Arbitration Agreement`).
- Use descriptive qualifiers instead of dates for study aids (e.g., `assignments`, `lektion 4 chat gennemgang ICL`).

## Folder rules
- `00_Master-Index` contains the global index and orientation notes.
- Each domain folder (10/20/30/40/50) stores its hub note, topics, and a `Cases/` subfolder where relevant.
- `60_Study-Aids` for syllabi, overview tables, lecture summaries.
- `70_Sandbox` captures raw stubs or drafts (not exam-ready).
- `90_Assets` holds media (`Images/`, `Canvas/`).
- `99_System/Templates` stores the standard note templates.

## Automation workflow
1. Create new notes via the templates in `/99_System/Templates`.
2. Run quality checks to ensure metadata + naming rules are applied before committing.
3. Update [[Master Index]] whenever a new hub or major topic appears.
4. Document review/approval outcomes in the note metadata (`tags: ["draft"]` vs `tags: ["approved"]`).

## Review cadence
- Weekly review of sandbox notes to determine whether they should be promoted, archived, or deleted.
- Monthly audit of cross-links to ensure the decision-tree and hub pages remain accurate.
