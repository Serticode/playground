# Bouncy Ripples

## 🚀 Live Demo

<https://dartpad.dev/?id=348db6f7f399b14195642a7199da0978>

### 📦 Source Code

<https://gist.github.com/Serticode/348db6f7f399b14195642a7199da0978>

### 🧠 Notes

- Three rings painted back to front (wave 3 → 0) so the newest ring always sits
  on top
- Each ring's value = wave index + animation.value — staggering them one full  
  cycle apart
- Radius = sqrt(canvasArea × value / 4) — grows outward from centre via
  square-root geometry
- Opacity = 1 − (value / 3), clamped — ring fades to nothing as it reaches the
  canvas edge
- CustomPainter repaint is driven by `super(repaint: animation)` — no setState
  needed
- AnimationController repeats on a 2-second cycle with no explicit curve —
  linear expansion
