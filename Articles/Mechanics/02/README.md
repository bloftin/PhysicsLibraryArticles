# 02 — Free-body diagram

PhysicsLibrary submission assets for **M02-02 Free-body diagram**.

## Files

- `M02-02_Free_Body_Diagrams.tex` — body source intended for the PhysicsLibrary encyclopedia entry editor.
- `preamble.tex` — minimal entry preamble used by the LaTeX source.

The earlier Markdown development draft remains at `../M02-02_Free_Body_Diagrams.md` for comparison/history. Future topic-specific diagrams, exercise data, or supplemental examples should be placed in this folder.

## Suggested PhysicsLibrary metadata

- **Title:** Free-body diagram
- **Entry type:** Definition
- **Primary PACS:** `45.20.Dd` — Newtonian mechanics
- **Additional PACS:** `45.50.Dd` — General motion
- **Synonyms:** free body diagram, force diagram, FBD
- **Defines:** system boundary, external force, internal force
- **Keywords:** Newton's laws, force, free-body diagram, normal force, friction, tension, spring force, drag force, equilibrium, circular motion
- **License intent:** CC BY-SA 4.0

## PhysicsLibrary-style decisions

The `.tex` file begins with the defined term emphasized using `\emph{}` and then develops the concept through sections, examples, common errors, exercises, and references. It is an entry body rather than a standalone document, so the source contains no `\documentclass` or title page.

The article uses ordinary LaTeX mathematics and simple array-based schematics instead of TikZ. This keeps the entry usable in PhysicsLibrary's default HTML-with-images renderer as well as page-image/PDF modes. External OER attribution is retained in a `thebibliography` section using `\PMlinkexternal`.
