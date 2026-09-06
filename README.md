# 二叉树树的博客 · leleblog

### ✨ 项目简介

一个基于 **Astro 5** 构建的现代化技术博客系统，是 [Fuwari](https://github.com/saicaca/fuwari) 的深度定制版（AcoFork 系），面向内容创作、展示与长期维护场景，部署于 **Cloudflare Pages**。在原版基础上扩展了全文检索、AI 摘要、维护脚本链路和多模块页面，拿来即用也能继续改造。

> [!CAUTION]
> 本仓库为深度定制版，包含最新文章与定制功能。若作为模板二次开发，建议具备一定 Astro / 前端工程经验。

### 🎨 主要特点

- ⚡ 高性能静态站点（Astro 5 + Svelte 5 交互岛）
- 🌗 响应式布局、全局深色主题与彩虹模式
- ✍️ Markdown / MDX 发布与增强渲染（行号、折叠、复制扩展）
- 🔍 全文检索、文章目录、阅读时长、更新提醒
- 🧩 多模块页面：归档、友链、赞助、画廊、文件索引、封面生成
- 📡 SEO 与分发：RSS、Sitemap、Robots、重定向
- 📊 页面访问统计与可视化入口
- 🧰 完整维护脚本：新建文章、图片清理、命名规范化、AI 摘要、差异更新

### 📦 包含模块

1. **博客核心**（`src/`）—— 页面、组件、内容集合与渲染链路
2. **内容管线**—— Remark / Rehype 扩展、Expressive Code 代码高亮
3. **维护脚本**（`scripts/`）—— 文章脚手架、图片清理、AI 摘要、差异更新等
4. **文档**（`docs/`）—— 定制点与二次开发说明
5. **部署配置**—— Cloudflare Pages 构建链路（`.github/` 工作流）

### 🛠️ 如何使用

1. 环境要求：Node.js 18+、pnpm 9.x
2. 安装并本地预览：

   ```bash
   pnpm install
   pnpm dev        # 本地开发
   pnpm build      # 构建生产版本
   pnpm preview    # 预览构建结果
   ```

3. 新建文章：使用 `scripts/` 中的文章脚手架，按 `frontmatter.json` 规范填写元数据
4. 部署：推送到 GitHub 后由 Cloudflare Pages 自动构建发布

### ❓ 效果演示

```bash
pnpm dev  →  http://localhost:4321
```

首页 · 归档 · 友链 · 画廊 · 文件索引等多模块页面，支持全文检索与深色彩虹主题切换；线上地址部署于 Cloudflare Pages。

### 🙏 贡献

模板底座来自 [Fuwari](https://github.com/saicaca/fuwari) 与 AcoFork 的定制工作，感谢上游作者。本仓库的定制功能欢迎 Issue 讨论；二次开发请先阅读 `docs/` 与 `CONTRIBUTING.md`。

> 本 README 按照 [App-Showcase-Template](https://github.com/yxs2003/App-Showcase-Template) 的展示流程编写。
