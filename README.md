# GitHub Pages 个人博客模板

这是一个免费的 GitHub Pages + Jekyll 个人博客模板，支持：

- Markdown 文章
- 图文内容
- LaTeX 公式
- 代码块
- 自定义样式

## 1. 创建仓库

在 GitHub 新建仓库，仓库名必须是：

```text
你的GitHub用户名.github.io
```

例如用户名是 `octocat`，仓库名就是：

```text
octocat.github.io
```

## 2. 上传模板

把本文件夹里的所有文件上传到这个仓库的根目录。

上传后，通常几分钟内就可以访问：

```text
https://你的GitHub用户名.github.io
```

## 3. 修改站点信息

打开 `_config.yml`，修改：

```yaml
title: "我的个人博客"
description: "记录学习、想法和研究笔记"
author: "你的名字"
url: "https://16752plus1.github.io"
```

## 4. 写新文章

在 `_posts` 文件夹新建 Markdown 文件，命名格式：

```text
年-月-日-文章英文或拼音标题.md
```

例如：

```text
2026-09-13-my-first-note.md
```

文章开头写：

```markdown
---
title: "文章标题"
description: "文章简介"
---

这里开始写正文。
```

## 5. 插入图片

把图片放到 `assets/images/`，然后在文章中引用：

```markdown
![图片说明]({{ '/assets/images/你的图片.png' | relative_url }})
```

## 6. 插入 LaTeX 公式

行内公式：

```markdown
这是行内公式 $E = mc^2$。
```

独立公式：

```markdown
$$
P(A mid B) = \frac{P(B mid A)P(A)}{P(B)}
$$
```

## 7. GitHub Pages 设置

如果页面没有自动发布，在仓库里进入：

```text
Settings -> Pages
```

选择从默认分支发布。用户站点一般使用 `main` 分支的根目录。
