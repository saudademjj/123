# 京城十日志 (Ten Days in Beijing - 沉浸式叙事交互实验)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![GSAP](https://img.shields.io/badge/GSAP-88CE02?logo=greensock&logoColor=white)](https://greensock.com/)
[![Interactive](https://img.shields.io/badge/Experience-Immersive-FF69B4)](https://saudademjj.github.io/beijing.html)

京城十日志是一个基于现代 Web 动画引擎构建的沉浸式叙事交互实验项目。项目旨在通过非线性的视觉流转与深度关联的滚动动效，将传统的城市游记升华为一场具备电影质感的数字艺术体验。

## 核心设计理念

- 深度交互式叙事: 突破传统的单向信息传递，利用横轴滚动与长焦视差效果，引导读者主动探索城市文化的深层脉络。
- 高级动效编排: 
    - 集成 GSAP 及其 ScrollTrigger 插件，实现像素级的关键帧控制与基于滚动的动画轨迹映射。
    - 结合流体视差 (Fluid Parallax) 与动态层深渲染，打造虚实结合的数字化视觉景观。
- 文本美学工程: 
    - 严谨的排版标准，深度结合 Noto 系列衬线与非衬线字体，平衡了信息的传递效率与视觉艺术感。
    - 自定义的高级光标交互体系，为细微的操作动作提供细腻的触觉化反馈。
- 全平台响应式兼容: 适配多样化的屏幕纵横比，确保在不同分辨率下都能保持叙事空间的完整性与艺术一致性。

## 技术栈

- 核心架构: HTML5 / CSS3 / ES6+ JavaScript
- 动画引擎: GSAP (GreenSock Animation Platform)
- 扩展插件: ScrollTrigger, ScrollToPlugin, TextPlugin
- 字体服务: Google Fonts (Noto Serif SC / Noto Sans SC)

## 项目结构

```text
.
├── index.html          # 沉浸式交互主页面入口
├── styles.css          # 全局视觉样式与动效契约定义
├── script.js           # 基于 GSAP 实现的动画核心引擎
└── README.md
```

## 本地预览

由于项目基于原生 Web 技术构建，可直接在主流浏览器中启动：

```bash
# 若已安装 serve
npx serve .
```

## 设计哲学
“将滚动视为时间轴的演进，将屏幕视为空间的延展。” 本项目强调技术对内容的深度赋能，致力于在数字媒介中重构“游记”的感知维度。

## 许可证
本项目采用 MIT License 协议。

---
Developed by [saudademjj](https://github.com/saudademjj)
