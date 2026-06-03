# Playground

A growing collection of Flutter creative coding experiments — animations, physics simulations, and visual engines — built live on [DartPad](https://dartpad.dev) and code hosted on [GitHub Gists](https://gist.github.com/Serticode).

## Contents

### Animations

| Experiment                                                      | Description                                                                                                          |
| --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| [Arc Dial](animations/arch_dial.md)                             | A scroll driven radial gauge with cosine faded ticks hanging from a large radius arc and a fixed gold centre marker. |
| [Animated Grid](animations/animated_grid.md)                    | A diagonal wave sweeps a cell grid, lighting each cell gold when it beats a per cell random threshold.               |
| [Bouncy Ripples](animations/bouncy_ripples.md)                  | Concentric ripple rings expand outward from centre via sqrt geometry, fading as they reach the canvas edge.          |
| [Linear Happiness Meter](animations/linear_happinness_meter.md) | A continuous 0–1 mood signal drives colour interpolation, arc progress, and animated emoji transitions.              |

### Visual Engines

| Experiment                                              | Description                                                                                                                            |
| ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| [Orbital Field Engine](visual_engines/orbital_field.md) | An interactive N-body gravity sandbox with suns, planets, moons, black holes, nebulae, orbit previews, presets, and JSON state export. |

## Structure

Each `.md` file is a self contained reference card — it links to the live DartPad demo and the source Gist, plus distilled implementation notes covering the math, rendering approach, and animation technique.

## License

- **Animations** — MIT. Completely free. Use them however you like. See [animations/LICENSE](animations/LICENSE).
- **Visual Engines** — Proprietary. Study and learn from the code, but do not use, copy, or reproduce it elsewhere. See [visual_engines/LICENSE](visual_engines/LICENSE).
