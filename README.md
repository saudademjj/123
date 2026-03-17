# 京城十日志

[English README](./README.en.md)

`京城十日志` 是一个纯前端静态展示页，围绕“北京十日深度文化行程”这一主题进行视觉化叙事。项目强调沉浸式首屏、滚动驱动动画、行程卡片编排和具有展陈感的页面节奏，适合做旅游专题页、作品集练习或静态页面设计参考。

## 功能特性

- 沉浸式首屏与加载过渡动画
- 行前筹谋信息卡片，覆盖预约、交通、餐饮、住宿与行李建议
- 10 天行程内容模块化展示
- 滚动进度条、数字计数器和视差感动画
- 自定义鼠标与悬浮交互效果
- 适配移动端浏览体验

## 技术栈

- `HTML5`
- `CSS3`
- `Vanilla JavaScript`
- `GSAP`（通过 CDN 引入 `ScrollTrigger`、`ScrollToPlugin`、`TextPlugin`）

## 本地预览

项目无需构建，直接启动静态服务器即可：

```bash
git clone https://github.com/saudademjj/123.git
cd 123
python3 -m http.server 8080
```

打开 `http://localhost:8080`

## 目录结构

```text
123/
├── index.html
├── styles.css
├── script.js
├── README.md
└── README.en.md
```

## 自定义建议

- 页面文案：修改 `index.html`
- 视觉主题：调整 `styles.css` 中的 `:root` 变量
- 动画节奏：编辑 `script.js` 中的 `gsap.timeline` 和 `ScrollTrigger` 配置

## 部署方式

可直接部署到任意静态托管平台：

- GitHub Pages
- Vercel
- Netlify
- Nginx 静态目录

## 使用提示

- 若动画未生效，请确认本地网络可以访问 GSAP CDN
- 不建议直接双击打开 `index.html`，最好通过本地 HTTP 服务访问

## 许可证

本仓库采用 MIT License，详见 [LICENSE](./LICENSE)。
