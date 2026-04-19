# Animated Grid

## 🚀 Live Demo

<https://dartpad.dev/?id=9e4ad6c4c9080aa86fda33d0de98aeae>

### 📦 Source Code

<https://gist.github.com/Serticode/9e4ad6c4c9080aa86fda33d0de98aeae>

### 🧠 Notes

- Diagonal wave sweeps left → right; diagIdx = (rows−1−row) + col
- Each cell has a random threshold (0.2–0.8) — wave must beat it to fire
- Crest cells (dist < 0.6) render at full gold; trailing cells at 72% opacity
- Cosine edge fade: same cos(norm × π/2)^1.4 formula as the arc dial
- Wave advances every 100 ms by 2 diagonal steps, wraps seamlessly
- Column count is responsive — recomputed from available width at 15px pitch
