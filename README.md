# Cosmic Horror Atlas

A curated reference corpus for cosmic horror craft analysis.

This repo serves two audiences in the same artifact:

1. **Curious readers** — a structured entry point into cosmic horror as a tradition. Not a reading list, not biographical encyclopedia. A map of the moves authors make and why those moves work.
2. **Claude Code** — a machine-retrievable knowledge base used during downstream creative work. Slash commands surface relevant prior art on demand.

The corpus may expand to other genres over time. Structure and schema are designed for that.

## What this is not

- Not a bibliography. Sources are referenced, not catalogued.
- Not plot summaries. Reading the original is not optional.
- Not biography. Authors exist here as collections of craft moves.
- Not quotations of in-copyright work beyond what analysis requires.

The content is original synthesis — that is what makes it useful both as a public reference and as a working substrate for creative projects in the genre.

## Structure

```
concepts/     # atomic craft ideas, one per file, tagged and cross-referenced
authors/      # index files per author, linking out to relevant concepts
techniques/   # specific craft moves (structural, prose-level, pacing, etc.)
principles/   # higher-order insights derived across multiple sources
```

The split between `concepts/`, `techniques/`, and `principles/` is a hierarchy of abstraction, not a strict taxonomy:

- **Concepts** — single ideas attributable to a tradition or author ("cosmic indifference as philosophical commitment").
- **Techniques** — concrete craft moves a writer can deploy ("withheld revelation", "geographic-scale dread").
- **Principles** — patterns observed across multiple authors and concepts ("dread compounds when scale outpaces comprehension").

When in doubt, write it as a concept and promote it later if a pattern emerges.

## Navigation

- Browse `authors/` to see what each writer is being read *for*, with links into concept files.
- Browse `concepts/` directly if you know the idea you want.
- Browse `principles/` for the big-picture takeaways.
- Use the slash commands (`.claude/commands/`) when working in Claude Code — see project `CLAUDE.md`.

## Curation discipline

This corpus is curated, not collected. See [MAINTENANCE.md](./MAINTENANCE.md) for pruning cadence and re-tag triggers. The goal is to avoid the "uncurated middle" — the failure mode where an archive grows past the point its owner can hold it in their head, and stops being useful.

## Status

Early. Schema and seed entries are in flux. Treat as a living document, not a finished reference.
