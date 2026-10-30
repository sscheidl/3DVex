# 3DVex v0.1 – implementation brief for Claude Code

## Goal
Build the smallest convincing UE5 desktop scene with two beakers and water transfer, while preserving a clean path to VR interaction.

## Sequence
1. Detect local UE5 and Blender installations; record exact versions. Do not assume installation paths.
2. Create a minimal UE5 project and a small laboratory scene using only self-authored geometry/materials.
3. Implement a reusable grabbable object interface and desktop mouse interaction.
4. Add two beakers with real-world scale and sensible pivot/grip behavior.
5. Implement simplified liquid state: source and target fill levels, tilt threshold, pour rate, valid receiving vessel and visual water stream. Prevent negative volumes and transfer outside valid geometry.
6. Make the liquid effect convincing without a computational fluid solver.
7. Test desktop interaction in Play-in-Editor and capture screenshots or a short recording for review.
8. Add documented scalability settings and a short reproducible test checklist.

## Architecture
Keep experiment state, interaction actions and presentation separate. Desktop and future VR controllers must call the same semantic actions (grab, release, set pose, begin/end pour as appropriate). Avoid hard-coded headset assumptions; prefer OpenXR for VR later.

## Explicit exclusions
No new experiments, progression system, corridor, doors, multiplayer, telemetry, AI tutor, complex menus, or full fluid simulation.

## Release gate
Stop after the two-beaker pouring demonstration meets the acceptance criteria in CONTRIBUTING.md. Ask before expanding scope.

## Publication safety
Public repository: no third-party code/assets/binaries, no copied examples, no proprietary plugins, no secrets. Check staged files and provenance before every push.
