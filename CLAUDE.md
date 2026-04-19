# CLAUDE.md — Cosmic Horror Atlas

## Purpose

This repo is a curated craft-analysis corpus. Two audiences:

1. Public readers exploring cosmic horror as a tradition.
2. Claude Code, retrieving prior art for downstream creative work in the genre.

When the user is working on a creative project and references this atlas, you are doing knowledge retrieval against a curated index — not free-form web search.

Project-specific operational details (which downstream projects, where they live, etc.) live in `CLAUDE.local.md` if present. That file is gitignored.

## Default behavior

- **Default `/effort` to `high`** for any task in this repo. Synthesis and craft analysis benefit from it.
- Read `README.md` and `MAINTENANCE.md` before adding entries — schema and discipline are documented there.
- When the entry count in `concepts/` + `techniques/` + `principles/` crosses 15, prompt the user for a pruning/re-tag pass per `MAINTENANCE.md`. Do not silently keep adding past 20 without surfacing this.

## Entry schema

Every file under `concepts/`, `techniques/`, or `principles/` follows this structure:

```markdown
# <Title — one idea, one file>

**Type:** concept | technique | principle
**Sources:** <author(s) and work(s) this draws from>
**Tags:** <kebab-case-tag>, <another-tag>
**Related:** [other-entry](../concepts/other-entry.md), [another](../techniques/another.md)

## Summary

Two to three sentences. Plain language. A reader who only reads this section should walk away with the core claim.

## Analysis

The substance. Original synthesis. Quote sparingly and only when a specific line is doing analytical work no paraphrase can do.

## Application

(Optional) How this informs working creative practice. Omit the section entirely if not applicable — do not leave a placeholder.
```

Author files under `authors/` are index-style, not full profiles:

```markdown
# <Author Name>

**Active:** <years or era>
**Tradition:** <e.g., American weird, British supernatural, Polish SF>

## Why they're in the atlas

One paragraph. What craft moves are they being read *for*. Not biography.

## Concepts drawing on this author

- [concept-title](../concepts/concept-title.md) — one-line hook
- ...

## Techniques drawing on this author

- [technique-title](../techniques/technique-title.md) — one-line hook
- ...
```

## Content rules

- **Atomic.** One idea per file. If a draft contains two claims, split it.
- **Original synthesis.** Not summary. Not biography. Not plot recap.
- **Copyright-conscious.** Public domain (Tolkien, Lovecraft, CAS, Hodgson, early Blackwood) tolerates more direct quotation. In-copyright work (Ligotti, Reynolds, Lem) gets paraphrase + short pointed quotes only.
- **Quotes must serve analysis.** A short quote followed by two paragraphs of analysis is the target shape. Long quotes followed by a sentence of commentary fail the standard and should be cut.
- **No filler.** If an entry can't pass "what new thing does this say," it doesn't ship.

## Cross-referencing

- Use relative markdown links: `[title](../concepts/title.md)`.
- Update the **Related** field on both ends of a new link.
- When creating a new concept, scan existing entries for cross-link opportunities — the corpus's value compounds with link density.

## Slash commands

Project commands live in `.claude/commands/`:

- `/author-profile <name>` — structured author breakdown
- `/concept-trace <concept>` — follow a concept across multiple authors
- `/cross-pollinate <a> <b>` — non-obvious connections between two entries
- `/find-precedent <problem>` — given a creative design problem, search the corpus
- `/technique-extract <description>` — identify the craft move underlying a passage

These commands operate against the corpus, not against the open web. If a query has no precedent in the atlas, say so explicitly rather than fabricating.

## Style

- Direct. No throat-clearing.
- Claims first, evidence second.
- "I" is fine when the analysis is genuinely the author's. Avoid academic distance.
- Match the user's voice profile (`~/code/github/R055LE/voice/voice-profile.md`) for any reader-facing prose.
