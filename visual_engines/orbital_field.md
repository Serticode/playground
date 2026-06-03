---
id: pad-orbital-field-engine
title: Orbital Field Engine
description: An interactive Flutter gravity sandbox where suns, planets, moons, black holes, and nebulae move through a softened N-body simulation with orbit previews, debug force vectors, trails, presets, and JSON state export.
tags: dartpad, flutter, physics, animation, custompainter, simulation
pinNumber: 4
createdAt: 2026-04-12
---

## 🚀 Live Demo

<https://dartpad.dev/?id=a33c2d934f4fdcc2cdff9725a08757ac>

### 📦 Source Code

<https://gist.github.com/Serticode/a33c2d934f4fdcc2cdff9725a08757ac>

### 🧠 Notes

- Gravity is modeled as a softened N-body simulation where every gravity enabled body pulls every other gravity enabled body
- Entity types include suns, planets, moons, black holes, nebulae, and background stars, with visual only bodies excluded from physics
- Orbital motion uses circular velocity seeding so newly placed planets and moons can enter stable looking paths
- Simulation advances with a fixed timestep accumulator for smoother, more predictable motion across frames
- Position and velocity updates using a velocity Verlet style integration step instead of naive frame by frame movement
- Adaptive sub steps help stabilize fast moving bodies and high acceleration moments near massive objects
- Orbit previews clone the current world, simulate a candidate body forward, and draw the projected path before committing it
- Trails are stored per body and rendered with fading strokes to make orbital history visible
- Debug mode visualizes velocity vectors and per source gravity indicators for the selected body
- Catalog objects include real world planets, moons, black holes, and nebulae with physical mass/radius metadata scaled into screen friendly simulation values
- Presets include Earth - Moon - Sun, binary stars, chaotic three body motion, and a compressed Solar System setup
- Rendering is handled through a CustomPainter layer with glowing suns, black hole rings, nebula gradients, shooting stars, trails, previews, and selection outlines
- UI composition is kept inside focused private widgets for banners, header chips, selection panels, preview panels, and the sandbox painter
