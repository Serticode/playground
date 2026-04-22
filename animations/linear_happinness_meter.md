# Linear Happiness Meter

## 🚀 Live Demo

<https://dartpad.dev/?id=0f57fa59ddad54a603ab0c8d3fd15186>

### 📦 Source Code

<https://gist.github.com/Serticode/0f57fa59ddad54a603ab0c8d3fd15186>

### 🧠 Notes

- Linear mood value (0.0 → 1.0) is treated as a continuous signal, not discrete steps
- Mood + interpolated color are derived via a typed record (MoodDerived), not loose variables
- Color blending uses segment based interpolation between adjacent mood stops
- Circular progress is rendered with a CustomPainter arc, sweeping clockwise from −π/2
- Progress animation is controller driven, tweening from previous → next value for smooth continuity
- Emoji transitions use AnimatedSwitcher (scale + fade) keyed by mood identity
- Label color and container glow react in sync with the interpolated active color
- UI composition avoids helper methods — built from private, focused widget classes
