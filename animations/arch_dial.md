# Arc Dial Animation

## 🚀 Live Demo

<https://dartpad.dev/?id=501e26f08708d23f7fd998ee3baf3d83>

### 📦 Source Code

<https://gist.github.com/Serticode/501e26f08708d23f7fd998ee3baf3d83>

### 🧠 Notes

- Radial geometry
- Gesture driven rotation
- Arc is the visible top of a large circle (r = 5000) whose centre sits below the viewport
- Ticks radiate inward (downward) from the arc — minor (24px) and major (48px)
  every 5th tick
- Cosine fade: ticks at the centre are fully opaque, edges fade to zero via
  `cos(norm * π/2)^1.4`
- Gesture driven rotation: 50px of scroll = 1 tick advance
- Gold centre marker is fixed — never scrolls, always at the midpoint
- Idle ticker advances the dial slowly when the page is not scrolling (0.0016  
   rad/sec)
