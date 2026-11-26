---
layout: default
title: 算記 FormuScript 教學
description: 算記（FormuScript）科學計算機與公式筆記的使用教學。
---

# 算記 FormuScript 教學

{{ site.apps.formuscript.tagline }}。從入門到進階的操作教學都放在這裡。

<p><a class="btn" href="{{ site.apps.formuscript.play }}">到 Google Play 下載</a></p>

<ul class="post-list">
{% for post in site.categories.formuscript %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="meta">{{ post.date | date: '%Y-%m-%d' }}{% if post.description %}　·　{{ post.description }}{% endif %}</span>
  </li>
{% endfor %}
</ul>

<p class="small"><a href="{{ site.apps.formuscript.privacy }}">算記隱私權政策</a></p>
