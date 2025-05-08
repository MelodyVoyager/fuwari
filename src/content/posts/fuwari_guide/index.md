---
title: fuwari guide
published: 2025-05-08
description: ""
image: "cover.jpeg"
tags: [guide, fuwari]
category: "guide"
draft: false
lang: ""
---

## 简介

Fuwari 是一个基于 Astro 和 Tailwind CSS 开发的现代化博客模板，具有流畅的动画效果和丰富的功能特性。本文档将帮助您快速上手使用 Fuwari 模板。

## 功能特性

- ✨ 基于 Astro 和 Tailwind CSS 开发
- �� 流畅的动画和页面过渡
- 🌓 亮色 / 暗色模式
- 🎯 自定义主题色和横幅图片
- 📱 响应式设计
- 🔍 搜索功能
- 📑 文章分类和标签系统
- ⏱️ 文章阅读时间估算
- 💻 代码高亮显示

## 快速开始

### 环境准备

1. 安装 pnpm

```bash
npm install -g pnpm
```

2. 克隆项目并安装依赖

```bash
git clone https://github.com/saicaca/fuwari
pnpm install
pnpm add sharp
```

## 开发命令

| 命令                       | 说明                                                 |
| :------------------------- | :--------------------------------------------------- |
| `pnpm new-post <filename>` | 创建新文章(文章将创建在 `src/content/posts/` 目录下) |
| `pnpm dev`                 | 启动本地开发服务器 (localhost:4321)                  |
| `pnpm build`               | 构建网站到 `./dist/` 目录                            |
| `pnpm preview`             | 本地预览构建后的网站                                 |
| `pnpm astro ...`           | 执行其他 Astro CLI 命令                              |

## 文章编写

### 文章前置信息

每篇文章都需要包含以下前置信息：

```yaml
---
title: 文章标题
published: 2024-01-01
description: 文章描述
tags: [标签1, 标签2]
category: 分类
draft: false
---
```

### 博客编写指南

#### Markdown 基础语法

1. 链接

- [链接文字](https://github.com/MelodyVoyager)
- [本地文档](fuwari_guide.html)
- [文档内跳转](#an-h2-header)

2. 脚注

这是一个脚注[^1]

[^1]: this is foot

3. 代码块

```python
def hello_world():
    print("hello world")
```

Note again how the actual text starts at 4 columns in (4 characters
from the left side). Here's a code sample:

    # Let me re-iterate ...
    for i in 1 .. 10 { do-something(i) }

1.  Dump everything in the pot and follow
    this algorithm:

        find wooden spoon
        uncover pot
        stir
        cover pot
        balance wooden spoon precariously on pot handle
        wait 10 minutes
        goto first step (or shut off burner when done)

    Do not bump wooden spoon or it will fall.

#### 数学公式

1. 行内公式 $\omega = d\phi / dt$

2. 块级公式

$$
\begin{equation*}
E = mc^2
\end{equation*}
$$

#### 提示框

:::note
普通提示
:::

:::tip
技巧提示
:::

:::important
重要提示
:::

:::warning
警告提示
:::

:::caution
注意提示
:::

> [!NOTE]
> The GitHub syntax is also supported.

> [!TIP]
> The GitHub syntax is also supported.

#### GitHub 仓库卡片

::github{repo="MelodyVoyager/fuwari"}

#### 视频嵌入

YouTube 视频

<iframe width="100%" height="468" src="https://www.youtube.com/embed/视频ID" title="YouTube video player" frameborder="0" allowfullscreen></iframe>

Bilibili 视频

<iframe width="100%" height="468" src="//player.bilibili.com/player.html?bvid=视频ID&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

## 部署指南

### 部署步骤

1. 编辑 `astro.config.mjs` 中的站点设置
2. 参考 [Astro 官方部署指南](https://docs.astro.build/zh-cn/guides/deploy/) 进行部署

## 许可证

MIT License
