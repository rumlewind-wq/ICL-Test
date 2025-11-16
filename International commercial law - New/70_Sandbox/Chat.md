---
title: "Chat"
topic: "chat"
type: doctrine
related: []
tags: []
---

You are an assistant operating on my GitHub repository that holds all my International Commercial Law (ICL) materials (lecture summaries, case notes, statute notes, etc.). Your task is NOT to invent new content, but to AGGREGATE and RESTRUCTURE existing content into a clean Obsidian-ready note structure.

Business objective:
Create one Markdown file per heading below and populate each file ONLY with relevant content you can find in the repo (lectures, notes, judgments, statute summaries, etc.). The result should be a high-level, centralised “hub” note for each theme, built entirely from material already in the repository.

Key constraints:
- Do not hallucinate or generate new legal analysis. Reuse and restructure content that already exists.
- Work only on files in this repo (primarily Markdown). If some content exists in text-like formats, you may reuse it, but ignore binaries you cannot read.
- Preserve legal precision: do not change legal meaning of any copied text.
- Where necessary, you may lightly normalise headings and bullet formatting, but do not rewrite the substance.
- Avoid duplication: if the same passage is reused in multiple places, centralise it once and cross-reference instead of copying it three times.
- Use Obsidian-style formatting: `#` headings and `[[wikilinks]]`.
- Where you aggregate from different files, add a short source pointer inline like `(source: [[filename]])` so I can trace origin.

File creation rules:
- Create one Markdown file per heading.
- File naming convention: `ICL - [Heading].md` (replace `/` with `-` or `–` if needed).
- Top of each file: use the exact heading in `# ...` format.
- Under each heading, structure content in bullet points and subheadings as needed.
- Group related material under logical subheadings (e.g. “Scope”, “Key rules”, “Cases”, “Instruments”) using `##` / `###`.

For each heading below:
1. Search the repo for existing content that matches the topic (keywords from heading, relevant regulations, conventions, and case names).
2. Extract and insert the relevant paragraphs, bullet points, case notes, and article summaries into the new file.
3. Maintain or add `[[wikilinks]]` to cases, regulations, and other topic notes that already exist or should obviously exist (e.g. `[[Brussels I Regulation (EU) 1215.2012]]`, `[[Rome I Regulation]]`, `[[New York Convention]]`, `[[Car Trim – Case C-381.08]]`, etc.).
4. If you find content already structured under a near-identical topic file, link to that file instead of duplicating the full text, and pull in only the key overview bullets.
5. If there is truly no relevant content in the repo for a given heading, create the file with the heading and insert a placeholder line: `- TODO: add content from lecture notes and case summaries (no existing material found in repo).`

Headings to implement:

1. `# 1. [[Introduction to International Commercial Law]]`
2. `# [[EU Private International Law – Foundations]]`
3. `# [[Jurisdiction in Civil and Commercial Matters (Brussels I / Brussels Ia)]]`
4. `# [[Recognition and Enforcement of Judgments (Brussels I / Brussels Ia)]]`
5. `# [[Complementary EU Instruments – European Procedures]]`
6. `# [[Additional EU Jurisdiction & Recognition Instruments]]`
7. `# [[Choice of Law for Contracts (Rome Convention / Rome I Regulation)]]`
8. `# [[Choice of Law for Non-Contractual Obligations (Rome II Regulation)]]`
9. `# [[Global Litigation Instruments – Hague 2005 & 2019 Conventions]]`
10. `# [[International Commercial Arbitration – Framework & Institutions]]`
11. `# [[The Arbitration Agreement]]`
12. `# [[Arbitration Procedure and Applicable Law]]`
13. `# [[The Arbitral Tribunal and Proceedings]]`
14. `# [[Arbitral Award|Awards]]`
15. `# [[Invalidity and Setting-Aside of Arbitral Awards]]`
16. `# [[Recognition and Enforcement of Arbitral Awards (New York Convention)]]`

Execution logic (high level):
- Step 1: Scan all Markdown files for keywords related to each heading (e.g. “Brussels I”, “jurisdiction”, “Rome I”, “Rome II”, “Hague 2005”, “Hague 2019”, “UNCITRAL Model Law”, “New York Convention”, “arbitration agreement”, “award”, “setting aside”, “enforcement”, etc.).
- Step 2: For each heading, collect relevant sections from the source files and paste them under the correct new `ICL - [Heading].md` file, grouped under sensible subheadings.
- Step 3: Insert `[[wikilinks]]` where appropriate (cases, regulations, conventions, major concepts), aligning with existing file names where possible.
- Step 4: Ensure each note is internally coherent (no half-sentences, no broken references) and avoid duplicated blocks across multiple headings.
- Step 5: Save all newly created notes in the same folder as my other ICL notes (or the project’s ICL notes folder if it is clearly identifiable).

Now perform this restructuring and file creation across the repo according to the above specification.
