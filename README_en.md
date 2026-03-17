<div align="center">
  English | <a href="./README.md">简体中文</a>
</div>

# Ten Days in Beijing (Immersive Narrative Interaction Experiment)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=flat-square&logo=greensock)
![Interactive](https://img.shields.io/badge/Experience-Immersive-FF69B4?style=flat-square)

"Ten Days in Beijing" is an interactive experimental project exploring the boundaries of "depth narrative" within digital media. As a specialized module of saudademjj.github.io, it reconstructs traditional travelogues into a cinematic digital experience with spatial depth, powered by the industry-standard GSAP animation engine.

## 🎨 Core Interaction Design

### 1. Pixel-Level Scroll Scheduling
The system eschews traditional discrete page scrolling in favor of non-linear animation mapping via **GSAP ScrollTrigger**:
- **Timeline Integration**: Vertical scroll distance is abstracted into a global animation timeline. The entry timing, movement paths, and opacity interpolation of every visual element are precisely driven by the scroll position.
- **Smooth Interpolation**: Implements a highly responsive feel using `scrub: true`, ensuring the user's scroll rhythm is perfectly synchronized with the animation state.

### 2. Fluid Parallax & Spatial Modeling
Constructs a profound visual space through multi-layer displacement techniques:
- **Multi-layer Parallax Streams**: By setting differentiated displacement ratios for the background (distant mountains), midground (historic architecture), and foreground (text and particles), the project simulates intense perspective depth within a flat viewport.
- **Visual Focus Steering**: Utilizes dynamic blur and scaling effects to guide the reader's eye across specific visual anchors according to the narrative flow.

### 3. Textual Aesthetics Engineering
- **Serif Atmosphere**: Deeply utilizes the Noto Serif SC typeface to create a sense of historical weight through stable Chinese glyphs.
- **Tactile Interaction**: Features a custom high-end cursor following logic. The cursor acts as more than just a pointer—it's an interactive anchor with physical inertia that generates subtle visual ripples in response to user movements.

## ⚙️ Technical Architecture

- **Core Engine**: Native JavaScript driven by the GSAP 3.12+ ecosystem.
- **Layout Contract**: Employs CSS Variables (Custom Properties) to coordinate parallax weights and color indices globally.
- **Performance Strategy**: Visual assets are WebP formatted, and `Intersection Observer` is used to optimize memory usage across long-axis content.

## 📂 Project Structure

```text
123/
├── index.html          # Main container for the immersive narrative
├── styles.css          # Global typography, parallax contracts, and motion layers
├── script.js           # Animation orchestrator and ScrollTrigger core
├── assets/             # Visual asset directory (parallax-ready slices)
└── README.md           # Technical specs and design documentation
```

## Preview
As this project is based on native Web tech, it can be launched via any static HTTP server:
```bash
npx serve .
```

## License
MIT License
