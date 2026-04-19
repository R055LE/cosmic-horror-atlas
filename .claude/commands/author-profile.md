---
description: Structured craft-analysis breakdown of an author from the atlas
---

You are operating against the cosmic-horror-atlas corpus. Read `CLAUDE.md` first if you have not in this session.

## Task

Produce a structured author profile for: **$ARGUMENTS**

Steps:

1. Check `authors/` for an existing index file for this author.
2. Read every concept, technique, and principle file linked from that index.
3. If no index exists, search `concepts/`, `techniques/`, and `principles/` for any entry citing this author in **Sources**.
4. Synthesize a profile structured as:

   - **Tradition / lineage** — where they sit in the cosmic horror genealogy (one paragraph).
   - **Signature moves** — the 3-5 craft choices that distinguish them, each with one supporting concept/technique link.
   - **What they pioneered vs. what they inherited** — separating innovation from execution-of-existing-form.
   - **What's worth stealing** — concrete, transferable craft moves for downstream work in the genre.
   - **What is not worth inheriting** — failure modes, dated assumptions, weaknesses to avoid.
   - **Open questions** — concepts about this author that the atlas has not yet captured.

5. End with a short list of suggested new entries to deepen coverage, if any.

Constraints:

- Original synthesis only. No biography filler.
- Cite only entries that exist in the corpus. If coverage is thin, say so.
- High effort. This is a synthesis task, not a lookup.
