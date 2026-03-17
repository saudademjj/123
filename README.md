# 京城十日志 (Ten Days in Beijing - 叙事交互实验)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![GSAP](https://img.shields.io/badge/GSAP-88CE02?logo=greensock&logoColor=white)](https://greensock.com/)
[![Interactive](https://img.shields.io/badge/Experience-Immersive-FF69B4)](https://saudademjj.github.io/beijing.html)

京城十日志是一个基于现代 Web 动画引擎构建的叙事交互实验。项目尝试通过非线性的视图切换与关联的滚动动效，将传统的城市游记转化为具备视觉深度的数字内容。

## 核心设计

- 交互式叙事: 突破单向展示，利用横轴滚动与视差效果，引导用户在不同页面间流转。
- 动效编排: 
    - 集成 GSAP 及其 ScrollTrigger 插件，实现基于滚动条位置的动画轨迹映射。
    - 结合流体视差效果，构建页面的空间深度。
- 排版与视觉: 
    - 结合 Noto Serif SC 与 Noto Sans SC 字体。
    - 自定义光标交互逻辑，为操作提供视觉反馈。
- 响应式适配: 针对多种屏幕分辨率进行布局兼容。

## 技术栈

- 架构: HTML5 / CSS3 / ES6+ JavaScript
- 动画引擎: GSAP
- 字体服务: Google Fonts (Noto 系列)

## 项目结构

```text
.
├── index.html          # 主入口
├── styles.css          # 全局样式
├── script.js           # 动画核心逻辑
└── README.md
```

## 本地预览

由于项目基于原生 Web 技术构建，可直接在主流浏览器中启动：

```bash
# 或使用 serve
npx serve .
```

## 许可证
MIT License
