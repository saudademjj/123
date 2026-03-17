<div align="center">
  <a href="./README_en.md">English</a> | 简体中文
</div>

# 京城十日志 (Ten Days in Beijing - 沉浸式叙事交互实验)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=flat-square&logo=greensock)
![Interactive](https://img.shields.io/badge/Experience-Immersive-FF69B4?style=flat-square)

京城十日志是一个探索数字媒介下“深度叙事”边界的交互实验项目。作为 `saudademjj.github.io` 的核心专项模块，项目旨在通过工业级 Web 动效引擎 GSAP，将传统的长轴游记内容重构为一场具备电影质感与时空张力的数字化交互体验。

## 核心设计理念

### 1. 像素级滚动调度逻辑
系统摒弃了传统的单向页面滚动，基于 **GSAP ScrollTrigger** 插件实现了非线性的动效映射。页面的滚动位置被抽象为动画的时间轴变量，精确控制着视觉元素的入场时机、运动轨迹与透明度渐变。

### 2. 流体视差与空间构建
利用流体视差技术 (Fluid Parallax)，通过对背景、中景与前景图层设置差异化的位移计算公式，在扁平的浏览器视口内构建出深邃的视觉空间感，增强了叙事内容的沉浸度。

### 3. 文本美学工程
- **排版标准**: 深度适配 Noto Serif SC 衬线字体，旨在通过严谨的中文字形营造具备历史厚重感的阅读氛围。
- **触觉化反馈**: 实现自定义的高级光标交互体系，为细微的鼠标位移提供细腻的视觉反馈，提升用户与内容间的交互张力。

## 技术架构简析

- **核心引擎**: GSAP 3.12+ / ScrollTrigger / ScrollToPlugin。
- **排版方案**: Google Fonts API 托管的 Noto 系列字体。
- **视觉优化**: 针对视差图层进行了 WebP 格式化处理与懒加载优化，确保在长轴内容下的加载平滑度。

## 项目结构图

```text
123/
├── index.html          # 沉浸式叙事主体容器实现
├── styles.css          # 全局排版规范、视差契约与关键帧样式定义
├── script.js           # 动效引擎核心逻辑与交互控制器
└── assets/             # 包含多层视差切片的视觉资产目录
```

## 预览方式
本项目基于原生架构，可直接通过静态 HTTP 服务器启动预览。

## 许可证
本项目遵循 MIT License 协议。
