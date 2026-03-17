# 京城十日志 (Ten Days in Beijing - 沉浸式叙事交互实验 / Immersive Narrative Interaction Experiment)

本项目是 `saudademjj.github.io` 的一个专项模块，独立于主作品集，旨在通过 GSAP 实现长轴滚动的视差叙事体验。

This project is a specialized module of `saudademjj.github.io`, independent of the main portfolio, aimed at exploring immersive parallax storytelling through GSAP-driven long-axis scrolling.

## 核心设计 / Core Design

- 沉浸式视差滚动 (Immersive Parallax Scrolling):
    - 基于 GSAP ScrollTrigger 插件实现的多层偏移。 / Multi-layer offsets using GSAP ScrollTrigger.
    - 针对长轴内容的视觉节奏控制。 / Visual rhythm control for long-axis content.

- 叙事布局 (Narrative Layout):
    - 结合排版美学与动态入场动效。 / Combining typographic aesthetics with dynamic entry animations.
    - 使用 Noto Serif SC 营造历史文化氛围。 / Noto Serif SC for cultural atmosphere.

## 技术栈 / Technical Stack

- 前端引擎: HTML5, CSS3, ES6+ JavaScript.
- 核心动画: GSAP 3.x, ScrollTrigger.
- 视觉资产: 视差图层与响应式图片流.

## 项目结构 / Project Structure

```text
123/
├── index.html          # 实验项目主入口 / Main entry
├── styles.css          # 视差与布局样式定义 / Styling
├── script.js           # 基于 GSAP 的滚动引擎 / GSAP engine
└── README.md
```

## 本地预览 / Preview

```bash
# 双击 index.html 或使用 http-server 预览
npx serve .
```

## 许可证 / License
本项目采用 [MIT License](LICENSE) 协议。 / This project is licensed under the MIT License.
