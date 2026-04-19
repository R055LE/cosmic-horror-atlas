# Maintenance

This corpus is curated, not collected. The discipline below exists to prevent the failure mode every personal knowledge base eventually hits: growing past the point its owner can hold it in their head, and quietly turning into a graveyard.

## The "uncurated middle" problem

A small archive (1-15 entries) is trivially knowable. A large, well-organized archive (100+) earns its weight through structure. The middle is where things rot — too big to remember, too small to have invested in retrieval scaffolding. Entries 15-50 are the danger zone.

The mitigation is not to slow down writing. It is to schedule deliberate consolidation passes.

## Pruning cadence

| Trigger | Action |
|---|---|
| Reaching 15-20 entries | First full pass: re-read every entry, prune the weak, retag, surface duplicates |
| Every ~25 entries after | Quick pass: scan titles + tags only, flag anything that no longer earns its slot |
| Every 6 months | Calendar pass regardless of count: tags drift, taxonomies stop fitting |
| Adding a new top-level directory | Re-evaluate whether existing entries belong in the new category |

Claude Code is instructed to prompt for the first pruning pass when entry count crosses 15. See `CLAUDE.md`.

## What earns an entry's slot

An entry survives a pruning pass if it satisfies at least one of:

- **Generative** — has produced at least one downstream insight, technique, or creative-work design decision.
- **Distinct** — captures a move not present elsewhere in the corpus.
- **Anchoring** — referenced by multiple other entries (high in-link count).
- **Foundational** — needed for a newcomer to make sense of the rest.

Entries that are merely *correct* but inert are removed or merged.

## Re-tag triggers

Tags drift faster than entries do. Review the tag set when:

- A tag has only one entry (over-specific — fold into a broader tag or drop)
- A tag has more than ~12 entries (under-specific — split)
- Two tags consistently co-occur (consider merging)
- A new entry needs a tag that doesn't quite fit any existing one (the existing taxonomy may be stale)

## Promotion / demotion

Entries can move between layers as understanding deepens:

- **concept → principle** when the same idea recurs across enough authors that it becomes a pattern, not an attribution.
- **technique → concept** if the move turns out to carry philosophical weight beyond the mechanical.
- **principle → concept** if a "principle" turns out to only describe one author's practice.

Movement is fine. Stagnation is the failure mode.

## What does not belong here

- Plot summaries
- Biographical material that isn't load-bearing for craft analysis
- Long quoted passages (short, pointed quotes serving analysis are fine — see `CLAUDE.md` on copyright posture)
- Reading notes that haven't been processed into a claim
- Entries written to be comprehensive rather than to be useful

If a draft can't pass the "what new thing does this say" test, it doesn't ship.
