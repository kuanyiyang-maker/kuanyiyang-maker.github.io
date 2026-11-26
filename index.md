---
layout: default
title: MagicSpark Studio App 教學
description: MagicSpark Studio 開發的 Android App：使用教學、操作技巧與隱私權政策。
---

# App 教學

這裡收錄 MagicSpark Studio 開發的 App 的使用教學與操作技巧。

<div class="cards">
  <section class="card">
    <h2>{{ site.apps.formuscript.name }}</h2>
    <p>{{ site.apps.formuscript.tagline }}</p>
    <p class="links">
      <a href="{{ '/formuscript/' | relative_url }}">看教學</a>
      <a href="{{ site.apps.formuscript.play }}">Google Play</a>
      <a href="{{ site.apps.formuscript.privacy }}">隱私權政策</a>
    </p>
  </section>
</div>

## 最新文章

<ul class="post-list">
{% for post in site.posts limit: 10 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="meta">{{ site.apps[post.categories.first].name }}　·　{{ post.date | date: '%Y-%m-%d' }}</span>
  </li>
{% endfor %}
</ul>
