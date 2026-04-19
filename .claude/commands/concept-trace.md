---
description: Follow a concept across multiple authors in the atlas
---

You are operating against the cosmic-horror-atlas corpus. Read `CLAUDE.md` first if you have not in this session.

## Task

Trace this concept across the corpus: **$ARGUMENTS**

Steps:

1. Search `concepts/`, `techniques/`, and `principles/` for entries semantically related to the concept (not just exact-string matches on the title).
2. For each match, identify which authors are cited and what variant of the concept they embody.
3. Produce a trace structured as:

   - **Canonical statement** — the cleanest articulation of the concept in the corpus, with link.
   - **Lineage** — chronological pass through how authors developed or mutated it. One paragraph per author.
   - **Variants** — distinct forms the concept takes (e.g., "concept X under cosmic-indifference framing" vs. "concept X under religious-horror framing").
   - **Tensions** — places where authors handle the concept incompatibly. These are often the most generative.
   - **Gaps in coverage** — authors or angles the corpus does not yet cover.

Constraints:

- Stay inside the corpus. Do not pull in external authors not represented in `authors/`.
- If the concept is thinly covered (fewer than 2 entries), report that and suggest 2-3 entries that would deepen the trace.
- High effort.
