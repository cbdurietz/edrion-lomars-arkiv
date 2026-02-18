# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Edrion Lomars arkiv** is a Swedish-language tabletop RPG campaign world presented as a scholarly archive. All content is written in Swedish. The repository is an Obsidian vault of markdown files – there are no build, lint, or test commands.

## Core Design Principle: The Archive Principle

This is not a traditional worldbook. Every text is framed as written by someone, preserved by someone, and interpreted by someone. Contradictions between documents are intentional features, not errors. There is no omniscient narrator voice. The namesake scholar Edrion Lomar is a collector, not an authority.

When creating or editing content, always consider:
- **Who wrote this?** Every document has an author with a perspective.
- **Why was it preserved?** Documents exist in the archive for a reason.
- **What is missing?** Gaps and omissions are deliberate.
- **Who would disagree?** Contradicting viewpoints are encouraged.
- **How could this be wrong?** Texts should suggest rather than explain definitively.

See `00-meta/vision.md` for the full design philosophy.

## Repository Structure

- `00-meta/` – Project framework, principles, glossary (vision.md is the key document)
- `01-arkiv/` – Polished archive material ready for use: fragments, chronicles, map notes
- `02-volymer/` – Compiled thematic volumes on specific regions (Ardenar in progress)
- `03-spelledare/` – Game master tools for using the archive in play
- `_arbetsmaterial/` – Internal working/development material (raw content, not published)
  - `01. Development/` – Active development organized by: Platser (Places), Personer (Characters), Folkslag (Peoples), Organisationer (Organizations), Religion, Väsen (Creatures), Material, Äventyr (Adventures)
- `assets/` – Images and maps

## Document Format

Archive documents in `01-arkiv/` use YAML frontmatter with these fields:

```yaml
titel:                  # Document title
typ:                    # Type (Arkivanteckning, Brev, Marginalanteckning, Randanmärkning, etc.)
forfattare:             # In-world author
roll:                   # Author's role/position
proveniens:             # Archive origin/location
datering:               # In-world dating
sprak:                  # Language of the document
tillforlitlighet:       # Reliability rating (medel, subjektiv, oklar)
relaterat_dokument:     # Related documents (Obsidian wiki-links)
kommentar:              # Archivist's commentary
```

## Working with Content

- The `_arbetsmaterial/` directory contains rough development notes. The `01-arkiv/` and `02-volymer/` directories contain structured, polished content.
- The project uses Obsidian wiki-links (`[[link]]`) for cross-references between documents.
- Place hierarchy follows: Aeteras → Aeterion → Prima → continent (e.g., Ardenar) → region/city.
- `struktur.txt` contains the planned directory layout for the project.
