<div align="center">
  <a href="./README.md">简体中文</a> | <a href="./README_en.md">English</a>
</div>

# 京城十日志 (Ten Days in Beijing - 沉浸式叙事交互实验 / Immersive Narrative Experiment)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=flat-square&logo=greensock)

京城十日志是一个探索“数字媒介下的深度叙事”的交互实验项目。项目作为 `saudademjj.github.io` 的核心子模块，旨在通过高级 Web 动效引擎 GSAP，将传统的长轴游记重构为一场具备电影质感与空间深度的视觉盛宴。

Ten Days in Beijing is an interactive storytelling project exploring "depth narrative in digital media." As a core sub-module of saudademjj.github.io, it aims to reconstruct traditional long-axis travelogues into a cinematic visual feast with spatial depth, powered by the GSAP animation engine.

## 核心动效与设计 / Core Animation & Design

### 1. 像素级滚动调度 (Pixel-level Scroll Orchestration)
- **GSAP ScrollTrigger**: 实现基于滚动位置的非线性动效映射，精确控制每一个视觉元素的入场时机与运动轨迹。 / Non-linear animation mapping based on scroll position.
- **多层视差流**: 利用流体视差技术 (Fluid Parallax)，通过不同背景层的差异化位移计算，构建深邃的视觉空间感。 / Multi-layer fluid parallax for spatial depth construction.

### 2. 文本美学与排版 (Textual Aesthetics & Typography)
- **字体工程**: 深度应用 Noto Serif SC 营造沉浸式的文化底蕴，配合自定义光标交互提升阅读反馈感。 / Noto Serif SC for cultural immersion with custom cursor feedback.
- **响应式叙事布局**: 采用流体容器确保叙事节奏在不同纵横比的屏幕下均能精准传达。 / Fluid layouts ensuring consistent narrative rhythm across devices.

## 技术架构 / Technical Stack

- **动效引擎**: GSAP (GreenSock Animation Platform) 3.12+ / ScrollTrigger.
- **基础标准**: 原生 HTML5 Semantic Tags / CSS 变量系统 / ES6+ Modules.
- **视觉优化**: 针对视差背景图层的预加载与 WebP 格式优化。 / Preloading & WebP optimization for visual assets.

## 项目结构图 / Project Structure

```text
123/
├── index.html          # 沉浸式叙事主体容器 / Main narrative container
├── styles.css          # 全局排版、视差契约与关键帧样式定义 / Styling & Layout
├── script.js           # 动画调度中心、ScrollTrigger 实例化逻辑 / Animation core
└── assets/             # 包含多层视差切片的视觉资源目录 / Visual assets
```

## 本地运行 / Local Setup
```bash
# 建议使用 http-server 或 VS Code Live Server
npx serve .
```

## 许可证 / License
本项目遵循 MIT License 协议。 / Licensed under the MIT License.
