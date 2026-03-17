<div align="center">
  <a href="./README_en.md">English</a> | 简体中文
</div>

# 京城十日志 (Ten Days in Beijing - 沉浸式叙事交互实验)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=flat-square&logo=greensock)
![Interactive](https://img.shields.io/badge/Experience-Immersive-FF69B4?style=flat-square)

京城十日志是一个探索数字媒介下“深度叙事”边界的交互实验项目。作为 `saudademjj.github.io` 的核心子模块，本项目旨在利用工业级动画引擎 GSAP，将传统的长轴图文记录重构为一场具备电影质感与空间深度的数字化叙事体验。

## 🎨 核心交互设计

### 1. 像素级滚动调度逻辑
系统摒弃了传统的离散式页面滚动，转而采用基于 **GSAP ScrollTrigger** 的非线性动效映射：
- **时间轴关联**: 页面的垂直滚动距离被抽象为全局动画的时间轴（Global Timeline）。每个视觉元素的入场时机、运动轨迹与透明度插值均由滚动位置精确驱动。
- **平滑插值**: 实现基于 `scrub: true` 的流畅反馈感，确保用户的滚动节奏与动效呈现完美同步。

### 2. 流体视差与空间建模
利用多图层位移技术构建深邃的视觉空间：
- **多层视差流**: 通过为背景（远山）、中景（古建筑）与前景（文字与颗粒）设置差异化的位移比率，在扁平的浏览器视口内模拟出极具纵深感的透视效果。
- **视觉焦点聚焦**: 通过动态模糊与缩放动效，引导读者的视线随叙事逻辑在不同视觉锚点间精准跳转。

### 3. 文本美学工程
- **衬线体意境**: 深度应用 Noto Serif SC 衬线字体，利用其稳重的中文字形营造历史厚重感。
- **触觉化交互**: 开发了自定义的高级光标跟随逻辑。光标不仅是一个指向器，更是一个具备平滑惯性的交互锚点，能够随用户的探索动作产生细腻的视觉涟漪。

## ⚙️ 技术架构分析

- **核心引擎**: 原生 JavaScript 驱动的 GSAP 3.12+ 生态。
- **布局契约**: 采用 CSS 变量 (Custom Properties) 统筹全页面的视差权重与色彩索引。
- **性能策略**: 针对高质量视觉资源进行了 WebP 格式化处理，并利用 `Intersection Observer` 优化长轴内容的内存占用。

## 📂 项目结构图

```text
123/
├── index.html          # 沉浸式叙事主体容器实现
├── styles.css          # 全局排版规范、视差契约与动效层级定义
├── script.js           # 动效引擎调度核心、ScrollTrigger 实例化中心
├── assets/             # 视觉资源目录 (经过视差分层处理的视觉切片)
└── README.md           # 技术规格与设计规范文档
```

## 预览方式
本项目基于原生 Web 技术构建，可直接通过静态 HTTP 服务器启动：
```bash
npx serve .
```

## 许可证
本项目采用 MIT License 协议。
