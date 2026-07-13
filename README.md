<div align="center">
  <h1 style="font-size: 3em; color: #6366f1; margin-bottom: 0.2em;">深渊园丁 · Minedensity</h1>
</div>

<img width="2560" height="1272" alt="image" src="https://github.com/user-attachments/assets/b724c06b-19ca-449a-958c-483c903f2ea0" />

> 叙事驱动型手绘交互艺术个人网站。

在浏览器里，种植一朵花，看太阳沉入地平线，往深渊的更深处走一走。
这座数字花园会随着你的停留慢慢生长。

🌐 线上地址：[minedensity.top](https://minedensity.top)

---

## 它是什么

不是博客模板，不是作品集陈列架。

它是一处**可以慢下来待一会儿的地方**——首页是一片会呼吸的花园，每一次点击都会留下痕迹；侧栏文字从叙事而非教学的角度写下技术札记；作品墙按"玩具 / 框架 / 山脉"三类摆开，记录从原型到产品之间的全部碎片。

你愿意点几下，就点几下；不愿意，**它不会催你**。

---

## 七个页面

| 路径 | 名字 | 一句话 |
|------|------|--------|
| `/` | 首页 | 一片会呼吸的花园，等待被种下第一朵花 |
| `/about` | 关于网站 | 四章散文，写给愿意慢下来的人 |
| `/projects` | 我的项目 | 玩具 / 框架 / 山脉——按思绪分类的作品墙 |
| `/projects/:slug` | 项目详情 | 进入某一个想法的内部 |
| `/blog` | 园丁手记 | 写作、复盘、生活碎片 |
| `/blog/:slug` | 文章 | 完整阅读模式 |
| `/recommendations` | 推荐 | 一些我反复回去看的东西 |

---

## 视觉与交互

- **手绘风**：所有插画来自 SVG 滤镜（噪点位移 + 笔触描边），没有用现成图标库
- **OKLCH 调色**：颜色空间统一，从调色板到 CSS 变量全程走 OKLCH
- **分层视差**：首页花园是 5 层 SVG 叠加 + Canvas 粒子，光标会留下痕迹
- **声音**：默认播放一段环境白噪音，可一键暂停
- **暗色 / 暗角**：纸张纹理 + 暗角滤镜贯穿全站
- **无障碍**：跳过链接、键盘可达、`prefers-reduced-motion` 适配

---

## 技术选型

| 类别 | 选型 |
|------|------|
| 框架 | Vue 3（Composition API + `<script setup>`） |
| 语言 | TypeScript |
| 构建 | Vite |
| 路由 | Vue Router |
| 状态 | Pinia |
| 样式 | Tailwind CSS 4 + 手写 CSS 变量 |
| 3D | Three.js（项目详情页封面） |
| 内容 | Markdown（YAML frontmatter） |
| 部署 | 静态导出 + Nginx |

> 代码不开源。这里只展示最终呈现。

---

## 本地预览

```bash
npm install
npm run dev
```

打开 `http://localhost:3000`。

构建生产版本：

```bash
npm run build
```

---

## 关于作者

- **GitHub**：[EVEDensity](https://github.com/EVEDensity)
- **邮箱**：18257184842@163.com

---

## 版权

© 2026 Density · 深渊园丁

本站内容仅供学习交流，转载请注明出处。

浙ICP备2026041074号
