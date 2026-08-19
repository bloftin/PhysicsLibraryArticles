# 01 — Mechanics learning path

PhysicsLibrary submission assets for **M00-01 Mechanics learning path**.

## Files

- `M00-01_Mechanics_Learning_Path.tex` — body source intended for the PhysicsLibrary encyclopedia entry editor.
- `preamble.tex` — minimal entry preamble used by the LaTeX source.

The earlier Markdown development draft remains at `../M00-01_Mechanics_Learning_Path.md` for comparison/history. Future topic-specific figures, exercises, or supporting data should be placed in this folder.

## Suggested PhysicsLibrary metadata

- **Title:** Mechanics learning path
- **Entry type:** Topic
- **Primary PACS:** `45.05.+x` — General theory of classical mechanics
- **Additional PACS:** `45.20.Dd`, `45.20.Jj`, `45.40.-f`, `45.50.-j`, `45.50.Pk`, `47.10.+g`
- **Keywords:** classical mechanics, Newtonian mechanics, analytical mechanics, Lagrangian mechanics, Hamiltonian mechanics, GRE physics, rigid body dynamics, oscillations, central force, non-inertial reference frame, fluid dynamics
- **License intent:** CC BY-SA 4.0

## PhysicsLibrary-style decisions

The `.tex` file is an **entry body**, not a standalone LaTeX document. It therefore has no `\documentclass`, title page, YAML front matter, or repository-only curriculum IDs in the rendered text. Internal PhysicsLibrary concepts are written as ordinary prose so Noosphere can auto-cross-reference them. External sources use `\PMlinkexternal` in the `thebibliography` environment.

Mermaid/TikZ was deliberately avoided in the submission body to preserve compatibility with PhysicsLibrary's default HTML-with-images renderer. The prerequisite map is expressed with ordinary LaTeX arrays, lists, and prose.
