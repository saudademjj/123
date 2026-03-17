<div align="center">
  English | <a href="./README.md">简体中文</a>
</div>

# Ten Days in Beijing (Immersive Narrative Interaction Experiment)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=flat-square&logo=greensock)
![Interactive](https://img.shields.io/badge/Experience-Immersive-FF69B4?style=flat-square)

"Ten Days in Beijing" is an interactive experimental project exploring the boundaries of "depth narrative" within digital media. As a specialized module of saudademjj.github.io, it aims to reconstruct traditional long-axis travelogue content into a cinematic digital experience with spatial depth, powered by the industry-standard GSAP animation engine.

## Core Design Philosophy

### 1. Pixel-Level Scroll Scheduling
Moving away from traditional one-way page scrolling, the system implements non-linear animation mapping based on the **GSAP ScrollTrigger** plugin. The page's scroll position is abstracted into a timeline variable, precisely controlling the entry timing, movement paths, and opacity gradients of visual elements.

### 2. Fluid Parallax & Spatial Construction
Utilizing Fluid Parallax techniques, the system applies differentiated displacement calculation formulas to background, midground, and foreground layers. This constructs a profound sense of visual space within the flat browser viewport, significantly enhancing the immersion of the narrative content.

### 3. Textual Aesthetics Engineering
- **Typography Standards**: Deeply optimized for the Noto Serif SC typeface to create a reading atmosphere with historical weight through rigorous Chinese glyphs.
- **Tactile Feedback**: Implements a custom high-end cursor interaction system that provides subtle visual feedback for fine mouse movements, increasing the interactive tension between the user and the content.

## Technical Architecture Overview

- **Core Engine**: GSAP 3.12+ / ScrollTrigger / ScrollToPlugin.
- **Typography**: Noto series fonts hosted via the Google Fonts API.
- **Visual Optimization**: Features WebP formatting and lazy-loading optimizations for parallax layers to ensure smooth loading performance across long-axis content.

## Project Structure

```text
123/
├── index.html          # Main container implementation for immersive narrative
├── styles.css          # Global typography specs, parallax contracts, and keyframe definitions
├── script.js           # Core animation engine logic and interaction controllers
└── assets/             # Visual asset directory containing multi-layer parallax slices
```

## Preview
As this project is based on a native architecture, it can be previewed directly via any static HTTP server.

## License
This project follows the MIT License protocol.
