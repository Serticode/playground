---
id: pad-pin-toggle-button
title: Pin Toggle Button
description: A custom micro interaction featuring a diagonal canvas curtain sweep and a dynamic multi stage spring bounce toggle animation.
tags: dartpad, animation, flutter, custom-painter, canvas, micro-interaction
pinNumber: 5
createdAt: 2026-09-19
---

## 🚀 Live Demo

<https://dartpad.dev/?id=09b5ec0fb0ae8a245817d7f93654e850>

### 📦 Source Code

<https://gist.github.com/Serticode/09b5ec0fb0ae8a245817d7f93654e850>

### 🧠 Notes

- **Diagonal Curtain Sweep:** Driven by a custom vector path in `_CurtainPainter` sliding from top right `(width, 0)` to bottom left `(0, height)` over the canvas
- **Dynamic Springs:** Uses a 4 part `TweenSequence` with `easeOut` and `easeOutBack` curves to achieve a playful pop, squash, and overshoot settling effect
- **State Selective:** `AnimationController` only plays `forward(from: 0)` when pinning; unpinning resets quietly without a bounce
- **Base Visibility:** Container background stays fixed at `10%` alpha so the diagonal sweep remains visually distinct throughout the animation
- **Zero Dependencies:** Built purely using Flutter primitives (`CustomPaint`, `ScaleTransition`, `TweenAnimationBuilder`)
