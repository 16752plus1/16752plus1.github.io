# GitHub Pages 图文内容上传指南

这个博客适合用 Markdown 写文章。推荐结构如下：

```text
.
├─ _posts/
│  └─ 2026-09-13-my-post.md
├─ assets/
│  ├─ css/
│  │  └─ style.css
│  └─ images/
│     └─ my-photo.jpg
├─ about.md
└─ index.md
```

## 上传一篇新文章

1. 打开 GitHub 仓库 `16752plus1/16752plus1.github.io`。
2. 进入 `_posts` 文件夹。
3. 点击 `Add file`，选择 `Create new file`。
4. 文件名使用 `年-月-日-英文标题.md`，例如：

```text
2026-09-13-study-note.md
```

5. 在文件开头写文章信息：

```markdown
---
layout: post
title: "我的第一篇图文笔记"
date: 2026-09-13
description: "这是一篇展示图片、公式和代码的文章。"
tags: ["学习", "笔记"]
---
```

6. 在下面继续写正文，最后点击 `Commit changes` 保存。

## 上传图片

1. 进入 `assets/images` 文件夹。
2. 点击 `Add file`，选择 `Upload files`。
3. 上传图片后点击 `Commit changes`。
4. 在文章里这样引用图片：

```markdown
![图片说明]({{ "/assets/images/my-photo.jpg" | relative_url }})
```

建议图片文件名只用英文、数字和短横线，例如 `reading-desk.jpg`，不要用空格。

## 图文文章模板

```markdown
---
layout: post
title: "文章标题"
date: 2026-09-13
description: "首页文章卡片里显示的摘要。"
tags: ["标签一", "标签二"]
---

这里写正文第一段。

![图片说明]({{ "/assets/images/example.jpg" | relative_url }})

这里写图片后的说明文字。

行内公式：$E = mc^2$

独立公式：

$$
P(A|B)=\frac{P(B|A)P(A)}{P(B)}
$$

```python
def hello(name):
    return f"Hello, {name}"
```
```

GitHub Pages 通常会在提交后 1 到 3 分钟自动更新。打开 `https://16752plus1.github.io/` 刷新即可看到新效果。
