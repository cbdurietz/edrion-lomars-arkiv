# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with content in this repository.

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

See `00. Arbetsmaterial/README.md` for the full design philosophy.

## Repository Structure

- `00. Arbetsmaterial/` – Internal working material. Mirrors the numbering of `01. Publicerat/` where applicable. `Filstruktur.md` inside describes the full structure and mappings.
- `01. Publicerat/` – Finished material organized as follows:
  - `10. Världsbok/` – Global world knowledge: cosmology, geography overview, common concepts. Written as encyclopaedia with no specific in-world author.
  - `11. Regioner/` – Regional modules in Hârn style: continent → region → city → village. Each level is a folder.
  - `20. Arkivet/` – Edrion Lomar's collection: fragments, chronicles, maps, letters. Organized by document type and provenance.
  - `30. Spelledarboken/` – Game master tools.
  - `80. Äventyr/` – Finished adventure modules.
  - `90. Regelbok/` – Rules (magic, peoples, professions, mechanics).

## Document Format

Archive documents in `01. Publicerat/20. Arkivet/` use YAML frontmatter with these fields:

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

- The project uses Obsidian wiki-links (`[[link]]`) for cross-references between documents.
- Place hierarchy follows: Aeteras → Aeterion → Prima → continent (e.g., Ardenar) → region/city.
- `00. Arbetsmaterial/Filstruktur.md` describes the full directory structure and the mapping between working material and published sections.
