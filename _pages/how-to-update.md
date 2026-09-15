---
permalink: /how-to-update/
title: "如何更新网站内容"
author_profile: true
---

本网站由 [Academic Pages](https://github.com/academicpages/academicpages.github.io) 模板搭建，内容以 Markdown 文件的形式存放在 GitHub 仓库 [yangfang0056/yangfang0056.github.io](https://github.com/yangfang0056/yangfang0056.github.io) 中。每次向仓库推送更新后，GitHub Pages 会自动重新构建网站，无需任何额外操作。

> 本页面由本人通过 AI 辅助（vibe coding）方式建站时编写，用于记录和说明网站内容的更新方法。

## 网站的文件结构

| 文件 / 目录 | 作用 |
|---|---|
| `_config.yml` | 网站全局配置（姓名、简介、链接、头像等） |
| `_pages/about.md` | 首页内容（个人介绍、教育、兴趣、动态） |
| `_pages/cv.md` | 个人 CV 页面 |
| `_pages/how-to-update.md` | 本页面（更新指南） |
| `_data/navigation.yml` | 顶部导航栏配置 |
| `images/` | 图片文件（头像等） |
| `files/` | 上传的附件（PDF、压缩包等） |
| `_posts/` | 博客文章（可选） |

## 更新方法一：直接在 GitHub 网页上编辑（推荐新手）

1. 打开仓库页面：[yangfang0056/yangfang0056.github.io](https://github.com/yangfang0056/yangfang0056.github.io)
2. 点击要修改的文件（例如 `_pages/about.md`）
3. 点击文件右上角的 **铅笔图标（Edit）**
4. 修改内容后，在页面底部填写提交说明（Commit message），例如 "update about page"
5. 点击绿色 **"Commit changes"** 按钮
6. 等 1-2 分钟，网站即自动更新

## 更新方法二：上传新文件

- 进入某个目录（如 `files/`），点击 **"Add file" → "Upload files"**
- 拖入文件后点击 **"Commit changes"**

上传到 `files/` 的文件可以通过 `https://yangfang0056.github.io/files/文件名` 访问。

## 更新方法三：用本地 Git 工具（进阶）

如果你安装了 Git，可以把仓库克隆到本地：

```bash
git clone https://github.com/yangfang0056/yangfang0056.github.io.git
```

修改文件后提交并推送：

```bash
git add .
git commit -m "更新内容说明"
git push
```

推送成功后，GitHub Pages 会自动重新构建网站（通常 1-3 分钟）。

## 常见更新场景

### 1. 更新个人简介 / 头像

- 简介：编辑 `_config.yml` 中的 `author.bio` 字段，或编辑首页 `_pages/about.md`
- 头像：把新照片上传到 `images/` 目录（覆盖 `profile.png`），或者修改 `_config.yml` 中 `author.avatar` 指向新文件

### 2. 添加一篇博客文章

在 `_posts/` 目录新建文件，命名格式必须为 `年份-月份-日期-标题.md`，例如：

```markdown
---
title: "我的第一篇博客"
date: 2026-09-15
---
这里是正文内容，支持 Markdown 语法。
```

### 3. 修改导航栏

编辑 `_data/navigation.yml`，增删 `main:` 下的条目即可。

### 4. 添加附件（PDF、PPT 等）

把文件上传到 `files/` 目录，然后可以在 Markdown 中用链接引用：

```markdown
[查看我的简历](/files/简历.pdf)
```

## 注意

- 修改 `_config.yml` 后，需要 1-3 分钟才能生效（GitHub Pages 自动构建）
- 如果页面显示异常，可以回到仓库的 **Actions** 标签页查看构建是否出错
- 仓库的所有修改都有历史记录，误操作可以随时回滚
