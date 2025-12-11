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

## ✨ 特点

- ✅ **白天** / **黑夜** 模式可用
- ✅ 极速的访问速度与优秀的 SEO
- ✅ 视图过渡动画（使用 ClientRouter）
- ✅ 支持文章全文搜索（Pagefind）
- ✅ 使用 [Tailwind CSS](https://tailwindcss.com/) 与 [daisyUI](https://daisyui.com/) 构建自适应页面
- ✅ RSS 订阅支持
- 🛠️ 博客易上手
  - 只需在 `Kael.config.yaml` 配置你的博客内容
- 🛠️ 本博客基于 [RyuChan](https://github.com/xz131714/RyuChan) 主题下进行修改  

## 📝 功能新增和修改（作者：Zayck）
- ✅ 修复**搜索功能**，精确呈现文章标题以及自动删除搜索历史
- ✅ 修改**导航栏背景**，由原来的毛玻璃透明效果改为纯色
- ✅ 修改导航栏的**搜索框位置**，让其贴近右边的光暗调节按钮
- ✅ 修改**搜索框内文字**的高对比度显示效果
- ✅ 删除~~番组组件、樱花特效~~组件
- ✅ 修改**About页面**，仿Markdown格式的页面浏览
- ✅ 修改**友链页面**，下方添加**评论组件**
- ✅ 修改**评论组件**为卡片式布局
- ✅ 修改**Rss页面**，暗黑模式下的美观页面浏览
- ✅ 修改**Umami 统计配置**一键开关显示博客访问量
- ✅ 修改**文章字体**、**标签字体**和**文章导航分页字体**，由原来的增大一号
- ✅ 修改**文章排版**，设置成两端对齐、两端缩进1个字符，更加美观的浏览体验
- ✅ 修改**高亮样式**，由原来的灰色改为主题蓝色，字体改为和文章字体一致
- ✅ 修改**引用代码块样式**，由原来的灰色改为主题蓝色
- ✅ 修改**代码块**样式，并修复点击复制按钮的交互功能
- ✅ 修改**网络卡片阴影效果**，由原来的三周环绕改为四周环绕
- ✅ 新增**license组件**的**打赏功能**
- ✅ 新增**license组件**分享按钮**微信**、**QQ**、**微博**方式
- ✅ 修改**license组件**间距
- ✅ 修改**鼠标样式**


## 😅 计划中……(期待大佬的参与)
- ❌ 动画效果：博客内跳转页面时太单调，想添加一些丝滑的过渡动画
- ❌ 音乐功能
- ❌ ……



## ✒️ 文章信息

|    名称     |   含义   | 是否必要 |
| :---------: | :------: | :------: |
|    title    | 文章标题 |    是    |
| description | 文章简介 |    是    |
|   pubDate   | 文章日期 |    是    |
|    image    | 文章封面 |    否    |
| categories  | 文章分类 |    否    |
|    tags     | 文章标签 |    否    |
|    badge    | 文章徽标 |    否    |
|    draft    | 草稿状态 |    否    |

> [!TIP]
>
> - 你可以通过把 `badge` 属性设置为 `Pin` 来置顶你的文章
> - 设置 `draft: true` 可将文章标记为草稿，草稿文章不会在列表显示

## ⬇️ 使用方法

1. 安装 pnpm 包管理器（如果你没有安装过的话）

```sh
npm i -g pnpm
```

2. 克隆项目

```sh
git clone https://github.com/zayck/Kael.git Kael
```

3. 进入项目文件夹

```sh
cd Kael
```

4. 安装依赖

```sh
pnpm i
```

5. 调试、运行项目

**首次运行或更新内容后**，请先执行 `search:index` 来生成搜索索引：

```sh
# 生成搜索索引以供开发时使用
pnpm run search:index

pnpm run dev
```

## 🔧 配置

Kael 使用 `Kael.config.yaml` 作为配置文件，你可以在此文件中配置网站的基本信息、导航栏、页脚等内容。

### 网站基本信息 (site)

```yaml
site:
  tab: Zayck # 浏览器标签栏上显示的文本
  title: Zayck # 网站的主标题
  description: A clean, elegant, and fast static blog template! # 网站描述，用于SEO
  language: zh # 网站的语言代码，如"en"表示英文，"zh"表示中文
  favicon: /goat.svg # 网站图标路径
```

### 主题设置 (theme)

```yaml
theme:
  light: winter # 浅色模式的主题，基于daisyUI的主题
  dark: dracula # 深色模式的主题，基于daisyUI的主题
  code: github-dark # 代码块的主题样式
```

- 主题基于 [daisyUI](https://daisyui.com/docs/themes/) 提供的主题选项
- 代码块主题使用 [Shiki](https://shiki.style/themes) 提供的样式

### 日期格式 (date_format)

```yaml
date_format: ddd MMM DD YYYY # 日期显示格式
```

### 菜单配置 (menu)

```yaml
menu:
  - id: home # 菜单项唯一标识符
    text: Home # 菜单显示的文本
    href: / # 链接地址
    svg: "material-symbols:home-outline-rounded" # 图标
    target: _self # 链接打开方式
```

每个菜单项包含以下属性：

- `id`: 唯一标识符
- `text`: 显示的文本
- `href`: 链接地址
- `svg`: 图标代码，使用 [Iconify](https://icon-sets.iconify.design/) 的图标集
- `target`: 链接打开方式(`_self`当前窗口或`_blank`新窗口)

#### 子菜单项 (subItems)

你可以通过添加 `subItems` 配置子菜单项，格式与主菜单项相同。

### 用户信息 (user)

```yaml
user:
  name: zayck # 用户名称
  site: "https://example.com" # 用户网站
  avatar: /profile.png # 用户头像
```

### 社交媒体配置 (social)

侧边栏和页脚可以配置不同的社交媒体链接：

```yaml
sidebar:
  social:
    - href: "https://github.com/zayck" # 链接地址
      ariaLabel: Github # 无障碍标签
      title: Github # 鼠标悬停时的提示
      svg: "ri:github-line" # 图标代码
```

### 图标设置 (icon)

Kael 使用 [Iconify](https://icon-sets.iconify.design/) 作为图标库。你可以在其网站上搜索你喜欢的图标，然后复制图标的代码到配置文件中的 `svg` 字段。

### 语言设置 (language)

Kael 支持多语言，通过以下方式配置：

1. 在 `Kael.config.yaml` 中设置网站默认语言：

```yaml
site:
  language: zh # 设置为 "zh" 使用中文，"en" 使用英文
```

2. 通过 `src/i18n/translations.yaml` 文件管理所有界面文本翻译：

```yaml
en: # 英文翻译
  label:
    noTag: No tags assigned
    tagCard: Tags
    # 其他英文标签...

zh: # 中文翻译
  label:
    noTag: 未分配标签
    tagCard: 标签
    # 其他中文标签...
```

#### 添加或修改翻译

要添加新的语言支持或修改现有翻译：

1. 在 `translations.yaml` 文件中添加新的语言代码和对应翻译，或修改现有翻译
2. 在 `Kael.config.yaml` 中更改 `site.language` 为你要使用的语言代码

## 🚀 自动更新

你可以使用我们提供的更新脚本保持项目与 Kael 的最新版本同步：

```sh
bash Kael.update.sh
```

该脚本将：

1.  **克隆最新版本** 的 Kael 仓库。
2.  **安全地更新** 你的项目文件，根据 `.updateignore` 文件添加和覆盖文件。
3.  **智能地删除** 官方仓库中已移除的文件，而不会影响你忽略的文件。
4.  **清理** 任何残留的空文件夹和临时文件。
5.  使用 `pnpm` **安装或更新** 依赖项。

## 👀 问题

如果你有任何问题或建议，可以通过提交 Issues 来反馈或同开发者交流！

