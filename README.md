<pre align="center">
一个简洁、优雅、快速的静态博客模板！🚀 使用 Astro 开发。
</pre>

<div align="center">
<img alt="Kael Logo" src="https://s1.vika.cn/space/2025/12/02/4967f95d7f9b4c9bae2368e9092796e8" width="280px">
</div>


[**🖥️ Kael Demo**](https://zayck-demo.pages.dev)
[**🖥️ 我的博客**](https://zayck.pages.dev)


## 📷 预览

![preview](https://s1.vika.cn/space/2025/12/02/7559170593c440c6a843cced5dd24c4a)


## ✨ 功能特性

### 核心功能

- [x] **Astro + Tailwind CSS** - 基于现代技术栈的超快静态站点生成
- [x] **流畅动画** - Swup 页面过渡动画，提供丝滑的浏览体验
- [x] **响应式设计** - 完美适配桌面端、平板和移动设备
- [x] **多语言支持** - i18n 国际化，支持简体中文、繁体中文、英文、日文、俄语
- [x] **全文搜索** - 基于 Pagefind 的客户端搜索，支持文章内容索引。同时支持 MeiliSearch 搜索引擎

### 页面组件
- [x] **留言板** - 支持留言页面，集成评论系统
- [x] **站点统计** - 显示文章、分类、标签数目、文章总字数、运行时长、最后更新时间
- [x] **站点日历** - 显示当月日历，以及当月的发布文章
- [x] **赞助页面** - 多种支付方式、收款码展示、赞助者列表、文章内赞助按钮
- [x] **友情链接** - 精美的友链展示卡片
- [x] **评论系统** - 集成 Twikoo、Waline、Giscus、Disqus、Artalk 评论系统
- [x] **访问量统计** - 支持调用 Waline、Twikoo 自带的访问量追踪

### 内容增强
- [x] **图片灯箱** - Fancybox 图片预览功能
- [x] **浮动目录** - 动态显示文章目录，支持锚点跳转，在侧边栏目录隐藏后显示
- [x] **侧边栏目录** - 动态显示文章目录，支持锚点跳转
- [x] **增强代码块** - 基于 Expressive Code，支持代码折叠、行号、语言标识
- [x] **数学公式支持** - KaTeX 渲染引擎，支持行内和块级公式
- [x] **Markdown扩展** - [Markdown extended features](https://github.com/saicaca/fuwari?tab=readme-ov-file#-markdown-extended-syntax)
- [x] **文章随机封面图** - 支持通过 API 获取随机封面图

### SEO
- [x] **SEO 优化** - 完整的 meta 标签和结构化数据
- [x] **RSS 订阅** - 自动生成 RSS Feed
- [x] **站点地图** - 自动生成 XML Sitemap，支持页面过滤配置


如果你有好用的功能和优化，请提交 [Pull Request](https://github.com/zayck/Kael/pulls)

## 🚀 快速开始

### 环境要求

- Node.js ≤ 22
- pnpm ≤ 9

### 本地开发部署

1. **克隆仓库：**
   ```bash
   git clone https://github.com/zayck/Kael.git
   cd Kael
   ```
   **先 [Fork](https://github.com/zayck/Kael/fork) 到自己仓库在克隆（推荐）**
   ```bash
   git clone https://github.com/you-github-name/Kael.git
   cd Kael
   ```
3. **安装依赖：**
   ```bash
   # 如果没有安装 pnpm，先安装
   npm install -g pnpm
   
   # 安装项目依赖
   pnpm install
   ```

4. **配置博客：**
   - 编辑 `src/config/` 目录下的配置文件自定义博客设置

5. **启动开发服务器：**
   ```bash
   pnpm dev
   ```
   博客将在 `http://localhost:4321` 可用

### 平台托管部署
- **可将博客部署至 Vercel, Netlify, GitHub Pages, Cloudflare Pages, EdgeOne Pages 等。**

   框架预设： `Astro`

   根目录： `./`

   输出目录： `dist`

   构建命令： `pnpm run build`

   安装命令： `pnpm install`


### 设置网站语言

要设置博客的默认语言，请编辑 `src/config/siteConfig.ts` 文件：

```typescript
// 定义站点语言
const SITE_LANG = "zh_CN";
```

**支持的语言代码：**
- `zh_CN` - 简体中文
- `zh_TW` - 繁体中文
- `en` - 英文
- `ja` - 日文
- `ru` - 俄文


### 配置文件结构

```
src/
├── config/
│   ├── index.ts              # 配置索引文件
│   ├── siteConfig.ts         # 站点基础配置
│   ├── profileConfig.ts      # 用户资料配置
│   ├── commentConfig.ts      # 评论系统配置
│   ├── licenseConfig.ts      # 许可证配置
│   ├── footerConfig.ts       # 页脚配置
│   ├── expressiveCodeConfig.ts # 代码高亮配置
│   ├── fontConfig.ts         # 字体配置
│   ├── sidebarConfig.ts      # 侧边栏布局配置
│   ├── navBarConfig.ts       # 导航栏配置
│   ├── friendsConfig.ts      # 友链配置
│   ├── sponsorConfig.ts      # 赞助配置
```
