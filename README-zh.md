# Rico Portfolio - 设计师个人作品集网站

一个基于 Astro 构建的现代化、高性能设计师个人作品集网站模板。采用复古蓝色主题，支持暗色模式，具有精美的动画效果和优秀的用户体验。

![Astro](https://img.shields.io/badge/Astro-5.15.4-FF5D01?logo=astro&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-4.1.14-38B2AC?logo=tailwind-css&logoColor=white)
![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)

## ✨ 特性

- 🚀 **基于 Astro** - 快速、轻量级的静态站点生成器
- 🎨 **现代化设计** - 复古蓝色主题，支持暗色/亮色模式切换
- 📱 **完全响应式** - 适配各种设备尺寸
- 🎭 **精美动画** - 使用 AOS 和自定义动画效果
- 📝 **博客系统** - 支持 MDX 格式的博客文章
- 🎯 **作品展示** - 优雅的作品集展示页面
- 🔍 **SEO 优化** - 内置 SEO 和社交媒体标签
- ⚡ **性能优化** - 图片优化、代码分割、懒加载
- 🌐 **国际化支持** - 易于扩展多语言支持

## 🛠️ 技术栈

- **框架**: [Astro](https://astro.build) 5.15.4 (兼容 v6)
- **样式**: [Tailwind CSS](https://tailwindcss.com) 4.1.14
- **动画**: [AOS](https://michalsnik.github.io/aos/)
- **物理引擎**: [Matter.js](https://brm.io/matter-js/)
- **内容管理**: MDX
- **类型检查**: TypeScript

## 📦 安装

### 使用包管理器

```bash

# 使用 pnpm (推荐)
pnpm install


# 使用 npm
npm install


# 使用 yarn
yarn install
```

### 环境变量配置

复制 `.env.example` 文件为 `.env` 并填写相应的配置：

```bash
cp .env.example .env
```

编辑 `.env` 文件，填入你的配置：

```env
# 站点 URL（可选，但有默认值 https://your-domain.com）
# 首次部署可以不设置，但建议尽快设置正确的域名以优化 SEO
PUBLIC_SITE_URL=https://your-domain.com

# 分析工具（可选）
PUBLIC_GA4_ID=your-google-analytics-id
PUBLIC_UMAMI_ID=your-umami-id
```

> **注意**：`PUBLIC_SITE_URL` 如果没有设置，会使用默认值 `https://your-domain.com`。虽然不会报错，但建议在部署后尽快设置正确的域名，以确保 sitemap、RSS feed 和 SEO 元标签正常工作。

## 🚀 开发

```bash
# 启动开发服务器
npm run dev
# 或
pnpm dev

# 访问 http://localhost:4321
```

## 📦 构建

```bash
# 构建生产版本
npm run build

# 预览构建结果
npm run preview
```

## 📁 项目结构

```
├── public/              # 静态资源
│   ├── assets/         # 图片、视频等资源
│   └── favicon.png     # 网站图标
├── src/
│   ├── assets/         # 源代码资源
│   ├── collections/    # 数据集合（作品、经历等）
│   ├── components/     # Astro 组件
│   │   ├── cards/      # 卡片组件
│   │   ├── sections/   # 页面区块组件
│   │   ├── ui/         # UI 组件
│   │   └── widgets/    # 小部件
│   ├── config/         # 配置文件
│   ├── content/        # MDX 博客内容
│   ├── layouts/        # 布局组件
│   ├── pages/          # 页面路由
│   ├── scripts/        # 脚本文件
│   └── styles/         # 样式文件
├── astro.config.mjs    # Astro 配置
├── tailwind.config.mjs # Tailwind 配置
└── package.json        # 项目依赖
```

## 🎨 自定义配置

### 修改网站信息

编辑 `src/config/site.js` 文件，修改网站的基本信息：

```javascript
export const siteConfig = {
  title: "Your Portfolio",
  author: "Your Name",
  url: "https://your-domain.com",
  // ... 更多配置
};
```

### 修改主题颜色

编辑 `src/styles/global.css` 文件中的 CSS 变量：

```css
@theme {
  --color-primary: #2d6dc3;
  --color-primary-dark: #3b7bd9;
  /* ... 更多颜色变量 */
}
```

### 添加作品

在 `src/collections/works.json` 中添加你的作品信息。

### 添加博客文章

在 `src/content/post/` 目录下创建新的 MDX 文件。项目使用 Astro v5 Content Layer API 和 `glob` 加载器来管理内容集合，确保与 Astro v6 兼容。

**注意**：此模板已完全升级到 Astro v5.15 标准，并兼容 Astro v6：
- ✅ 使用新的 Content Layer API (`glob` 加载器)
- ✅ 使用 `entry.id` 替代已弃用的 `entry.slug`
- ✅ 使用 `render(entry)` 替代已弃用的 `entry.render()`
- ✅ 使用 `import.meta.env` 替代 `process.env`
- ✅ 使用 `import.meta.glob()` 替代已弃用的 `Astro.glob()`
- ✅ 所有 `getStaticPaths()` 的 params 都是字符串类型（v6 要求）


## 使用素材

- **Programming Sticker**: [Figma rogramming-sticker-1-0](https://www.figma.com/community/file/1392100849031958853/programming-sticker-1-0)
- **Bento Cards**：[Figma Bento Cards](https://www.figma.com/community/file/1231184483170475120)
- **Social Cards**: [Figma Bento 2.5d](https://www.figma.com/community/file/1232620929235403629/bento-2-5d-widgets)

## 📧 联系方式

- **作者**: Ricoui
- **博客**: [ricoui.com](https://github.com/kei-kez)
- **邮箱**: hello@ricoui.com
- **Twitter**: [@kez](https://x.com/ricouii)
- **GitHub**: [@kei-kez](https://github.com/kei-kez)


## 💡 其他产品

-  **Rico Blog** - 开源 :  [https://github.com/kei-kez/public-portfolio-site](https://github.com/kei-kez/public-portfolio-site)

- **OG Gallery**: [ricoog.com](https://ricoog.com/)


## 🙏 致谢

- [Astro](https://astro.build) - 优秀的静态站点生成器
- [Tailwind CSS](https://tailwindcss.com) - 实用优先的 CSS 框架


## 📝 更新日志

### 最新更新 (2024)

- **升级到 Astro 5.15.4** - 完全符合 Astro v5.15 标准，兼容 Astro v6
- **内容集合升级** - 使用新的 Content Layer API，移除了所有旧版 API
- **API 现代化** - 所有已弃用的 API 已更新为最新标准
- **性能优化** - 优化了构建和运行时性能

查看 [CHANGELOG.md](CHANGELOG.md) 了解完整版本更新历史。


## 关于作者

我是Rico，网页/UI设计师，热衷于做些有趣和创意的作品。拥有 UI/UX 设计工作经验，目前专注于网页设计和视觉落地，以及开发项目探索。我平时在博客<a href="https://ricoui.com/" target="_blank">Rico's Blog</a>更新内容。也可以关注我的小红书 [@Rico的设计漫想](https://www.xiaohongshu.com/user/profile/5f2b6903000000000101f51f) 和 推特 [@ricouii](https://x.com/ricouii).

或者添加我的微信，交个朋友

<img src="https://ricoui.com/assets/wechat.png" alt="ricocc-wechat" width="280" height="auto" style="display:inline-block;margin:12px;">


## 💜 支持作者


如果觉得有所帮助的话，一点点支持就可以大大激励创作者的热情，感谢！

<img src="https://ricoui.com/assets/zanshangma.jpg" alt="ricocc-wechat" width="280" height="auto" style="display:inline-block;margin:12px;">


---

⭐ 如果这个项目对你有帮助，请给一个 Star！
