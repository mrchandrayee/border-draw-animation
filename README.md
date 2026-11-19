# Border Draw | Animation

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://mrchandrayee.github.io/border-draw-animation/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org) [![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

A responsive, runnable HTML/CSS recreation of the three border effects shown in the uploaded 8.04-second screen recording.

## Effects
1. **Border Draw** — on hover/focus, the top/right and bottom/left border strokes are revealed in a staggered sequence.
2. **Perpetual Draw** — an animated gradient stroke continuously loops around the card; no hover is required.
3. **Corner Sweep** — a gradient highlight sweeps around the card border on hover/focus.

## Source code actually legible in the video

The screen shows this HTML line:
```html
<div class="card draw-border">
```

The CSS base `.card` block is legible:
```css
.card {
  width: 320px;
  background: rgba(15, 25, 35, 0.65);
  backdrop-filter: blur(8px);
  border-radius: 24px;
  padding: 2rem 1.5rem;
  text-align: center;
  box-shadow: 0 25px 40px rgba(0, 0, 0, 0.3);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  position: relative;
  cursor: pointer;
}
```
The screen's third card title is **Corner Sweep**. The second card is visibly titled **Perpetual Draw** (not “Perpetual Glow”). The video states that the first draws from corners, the second loops continuously, and the third sweeps a glowing gradient across all four edges.

## Run
No dependencies or build tools are needed:
```bash
python3 -m http.server 8000
```
Open http://localhost:8000.

## Files
- `index.html` — semantic card markup and visible source-code panels
- `styles.css` — responsive styling and three CSS-only border animations

## Accuracy note
This 8-second recording shows only one HTML snippet and the base `.card` CSS block clearly enough to transcribe. It does not expose the full original HTML/CSS source for the three effects. The two visible snippets above are transcribed from the screen; the remaining implementation is a complete recreation based on the visual behavior and captions, not the original creator's complete source code. No JavaScript is required for these hover/focus animations.

## 👨‍💻 Author

**mrchandrayee** · [GitHub](https://github.com/mrchandrayee)

## 📄 License

[MIT License](./LICENSE)
