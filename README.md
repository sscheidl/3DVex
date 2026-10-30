# 3DVex

Experimental 3D chemistry laboratory prototype using Unreal Engine 5.

## Scope: v0.1 feasibility prototype

One small laboratory room, one workbench, two transparent beakers and a visually convincing water-pouring interaction. On desktop, users can pick up, move, tilt and put down a beaker using mouse controls. No physically accurate fluid simulation is required.

**Stop condition:** v0.1 is complete when pouring from one beaker into the other works reliably and looks convincing. No doors, additional experiments, curriculum management, multiplayer or learning platform in this milestone.

## Design principles

- **Desktop first, VR-ready by design:** Keep experiment logic independent from input devices. Mouse/keyboard and future OpenXR controller interactions invoke the same object actions.
- **VR comfort:** Do not force camera transitions or movement in VR. Use real-world scale and plausible grasp points.
- **Scalable visuals:** Provide low, medium and high graphics profiles; visual quality must not alter experiment outcomes.
- **Pragmatic physics:** Prefer predictable state-based liquid transfer with visual effects over expensive full fluid simulation.
- **Modular future:** Avoid hard-coding a single device type into input handling, without building a generic framework prematurely.

## Development stack

- Unreal Engine 5 (locally installed, version to be pinned after setup)
- C++ and/or Blueprints for runtime interaction
- Unreal Python Editor Scripting for repeatable editor automation
- Blender for self-created models and assets
- OpenXR for future VR support, initially targeting an Oculus Rift S for testing

Claude Code may automate project setup and testing locally. Verify actual editor/runtime behavior with human review or captured screenshots; successful compilation alone is not acceptance.

## Repository rules

This public repository contains **only our own project source code and self-created assets**. Do not commit third-party source code, proprietary binaries, downloaded models, textures or plugins, Unreal Engine files, or locally generated builds. External dependencies must remain external. Consult [CONTRIBUTING.md](CONTRIBUTING.md).

## Current status

Planning scaffold only. No Unreal project or functioning simulation has been committed yet.

## Related project

[SiVex](https://github.com/sscheidl/SiVex) — separate browser-based virtual chemistry experiments.
