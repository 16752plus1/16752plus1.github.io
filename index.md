---
layout: default
title: 首页
---

<section class="intro">
  <p class="eyebrow">Personal Blog</p>
  <h1>你好，我在这里记录想法、学习和作品。</h1>
  <p>这是一个基于 GitHub Pages 的免费个人博客模板，支持 Markdown、图片、代码高亮和 LaTeX 公式。</p>
</section>

<section class="post-list" aria-label="文章列表">
  <h2>最新文章</h2>
  {% for post in site.posts %}
    <article class="post-item">
      <a href="{{ post.url | relative_url }}">
        <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
        <h3>{{ post.title }}</h3>
        {% if post.excerpt %}
          <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
        {% endif %}
      </a>
    </article>
  {% endfor %}
</section>
