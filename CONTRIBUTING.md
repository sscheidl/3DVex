# Development and publication rules

This repository is **public**. Treat every commit as immediately published.

1. Commit only source code authored for 3DVex by us or our authorized coding assistants, and assets created by us for this project.
2. Never copy code from Maroon, FarmasiaVR, Unreal Engine, tutorials, marketplace packages or other external repositories into 3DVex. Use such projects for conceptual and technical research only.
3. Never commit third-party executables, DLLs, plugins, firmware, prebuilt binaries, downloaded 3D models, textures, sound files or proprietary project files.
4. Self-authored Unreal binary asset files (.uasset/.umap) may be committed when necessary; verify provenance before each commit.
5. Do not commit secrets, tokens, personal information, local paths, caches, generated builds or engine installation files.
6. Reference external dependencies by documentation and installation instructions rather than vendoring them.
7. Check git status and staged changes before pushing. When origin or rights are uncertain, **do not commit**.
8. Use the repository's Unreal .gitignore; keep large generated artifacts out of Git history.
9. Avoid GitHub Actions workflows unless they provide clear value. Do not duplicate push and pull_request checks for the same commits.
10. Keep the v0.1 milestone deliberately small. Do not add experiments, menus, doors or learning management without an explicit scope decision.

## Acceptance criteria for v0.1

- Room and table render correctly in a packaged or editor-playable desktop scene.
- Two self-created beakers are visible, one initially containing water.
- Mouse interaction can grasp, lift, tilt and place the source beaker.
- Water transfers visually and the displayed fill levels change plausibly.
- Interaction logic is separated from desktop input to permit future OpenXR controller bindings.
- A lower-quality graphics configuration works without changing simulation logic.
- A short reproducible manual test procedure is documented.

VR operation is a later verification milestone, not a prerequisite for closing v0.1.
