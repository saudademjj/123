# 京城十日志（静态网页）

一个纯前端静态页面项目，主题是「北京十日深度文化行程」。页面包含沉浸式视觉设计、滚动动画、行程卡片与统计计数器，适合用作旅游展示页或视觉练习作品。

## 主要功能

- 沉浸式首屏（加载动画、渐入文案、滚动引导）
- 行前筹谋信息卡（预约、交通、餐饮、住宿、安全、行李）
- 10 天行程卡片（按天展示，含亮点与建议）
- 滚动进度条、数字计数动画、视差背景
- 自定义鼠标光标与交互悬浮效果
- 全中文内容与移动端适配

## 技术栈

- `HTML5`
- `CSS3`（变量、渐变、响应式布局）
- `Vanilla JavaScript`
- `GSAP`（通过 CDN 引入）
  - `gsap`
  - `ScrollTrigger`
  - `ScrollToPlugin`
  - `TextPlugin`

## 本地运行

本项目无构建步骤，直接启动静态服务器即可：

```bash
git clone https://github.com/saudademjj/123.git
cd 123
python3 -m http.server 8080
```

浏览器访问：`http://localhost:8080`

## 目录结构

```text
123/
├── index.html     # 页面结构与内容
├── styles.css     # 样式与主题变量
├── script.js      # 动画与交互逻辑
└── README.md
```

## 定制指南

- 修改行程内容：编辑 `index.html` 中各 `day-card` 区块。
- 修改视觉风格：编辑 `styles.css` 顶部 `:root` 颜色变量。
- 修改动画节奏：编辑 `script.js` 中 `gsap.timeline` 与 `ScrollTrigger` 配置。

## 部署建议

可直接部署到任意静态托管平台：

- GitHub Pages
- Vercel
- Netlify
- Nginx 静态目录

## 常见问题

1. 页面动画未生效
- 检查网络是否可访问 CDN（GSAP 依赖在线加载）。

2. 本地双击 `index.html` 打开效果异常
- 建议使用本地 HTTP 服务（如 `python3 -m http.server`），不要直接用 `file://`。

## 许可证

当前仓库未显式提供 License 文件，如需开源发布建议补充 `LICENSE`。
