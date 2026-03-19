<div align="center">
  <a href="./README_en.md">English</a> | 简体中文
</div>

# 京城十日志 -- 沉浸式艺术体验网页

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=flat-square&logo=greensock)

一个以「京城十日志」为主题的沉浸式静态网页，记录北京十日深度文化探索之旅。项目在设计上融合现代艺术审美与沉浸式交互体验，完全基于原生 Web 技术栈构建，不依赖任何前端框架，通过 GSAP 动画引擎实现电影级的视觉叙事效果。

## 设计理念

本项目将旅行记录提升为一种视觉叙事体验。不同于传统的图文博客，页面通过精心编排的动画时序、滚动驱动的内容揭示和电影级的过渡效果，让浏览者仿佛身临其境地跟随作者走过北京的每一天。

## 核心交互功能

### 电影级开场

- 全屏加载过渡画面：衬线字体「京城十日志」标题渐显，营造仪式感
- 加载完成后平滑过渡到主内容区域
- 首屏 Hero 区域配合背景动画与「开启旅程」CTA 按钮

### 滚动驱动叙事

- 页面顶部实时阅读进度条，反馈当前浏览位置
- 基于 GSAP ScrollTrigger 的区块渐入动画：内容随滚动逐步揭示
- 各章节（筹谋、数据、行程）通过导航栏平滑滚动定位

### 自定义光标系统

- 双层光标设计：外圈（cursor）+ 内点（cursor-dot）
- 光标跟随鼠标移动，带有平滑的延迟跟随效果
- 在交互元素（链接、按钮）上产生形变反馈

### 动态数据展示

- 关键数字（行程天数、景点数量、步行距离等）在进入视口时触发从零到目标值的动态递增动画
- 数据计数器配合缓动函数，呈现自然的数值变化节奏

### 卡片式行程编排

- 10 天行程以响应式卡片网格布局呈现
- 每张卡片包含日期、主题、行程亮点
- 卡片悬浮时的自定义视觉反馈

## 页面结构

页面由以下主要章节组成：

- Hero 区域：全屏标题与背景动画，引导用户开始浏览
- 行前筹谋：旅行准备的关键要素与实用建议
- 数据纵览：行程关键数据的动态可视化展示
- 十日行程：逐日行程的卡片式详细编排

## 技术栈

- HTML5：语义化标签结构，注重文档可访问性与 SEO
- CSS3
  - 原生自定义属性（CSS Variables）统一主题管理
  - Flexbox 与 Grid 混合布局
  - 响应式媒体查询适配多种屏幕尺寸
  - 自定义滚动条样式
  - 过渡与关键帧动画
- 原生 JavaScript
  - DOM 操作与事件监听
  - Intersection Observer API 检测元素可见性
  - 自定义光标位置计算与跟随逻辑
  - 数据计数器递增算法
- GSAP（GreenSock Animation Platform）
  - 通过 CDN 引入的工业级动画引擎
  - ScrollTrigger 插件：滚动位置驱动的动画触发与时间线控制
  - 丰富的缓动函数预设（easing）实现自然运动曲线
- Google Fonts
  - Noto Sans SC：正文无衬线字体
  - Noto Serif SC：标题衬线字体，营造文化质感

## 文件结构

```text
123/
├── index.html       # 主页面：完整的内容结构与语义化标记
├── styles.css       # 全局样式：CSS 变量、布局、响应式规则、动画
├── script.js        # 交互逻辑：GSAP 动画、ScrollTrigger、计数器、光标
└── README.md        # 项目说明文档
```

## 本地预览

无需任何构建工具或依赖安装，使用 Python 自带的 HTTP 服务器即可预览：

```bash
git clone https://github.com/saudademjj/123.git
cd 123
python3 -m http.server 8080
```

在浏览器中访问 `http://localhost:8080` 即可查看完整效果。

也可以使用其他静态文件服务器：

```bash
# 使用 Node.js 的 serve
npx serve .

# 使用 PHP 内置服务器
php -S localhost:8080
```

## 定制指南

本项目适合作为旅行记录、活动专题页或个人叙事页面的模板：

### 内容修改
- 编辑 `index.html` 中的文本内容、章节结构和卡片数据
- 替换 Hero 区域的标题与副标题
- 调整行程卡片的天数与内容

### 主题配色
- 修改 `styles.css` 顶部 `:root` 中的 CSS 变量
- 调整背景色、文字色、强调色等主题参数

### 动画调整
- 在 `script.js` 中修改 GSAP 时间线配置
- 调整 ScrollTrigger 的触发位置与动画持续时间
- 修改缓动函数（easing）改变动画节奏

### 字体替换
- 在 `index.html` 的 `<head>` 中替换 Google Fonts 链接
- 在 `styles.css` 中更新对应的 `font-family` 声明

## 浏览器兼容性

- 推荐使用现代浏览器（Chrome、Firefox、Safari、Edge 最新版本）
- GSAP ScrollTrigger 需要支持 Intersection Observer API
- 自定义光标效果在触屏设备上自动隐藏

## 许可证

MIT License
