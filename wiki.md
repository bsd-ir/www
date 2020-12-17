---
layout: page
title: Wiki - ویکی
permalink: /wiki/
---

<h2>Wiki - ویکی</h2>

<div>&nbsp;</div>

<h3>ویکی فارسی</h3>

<ul class="post-list">
  {% for post in site.wiki_fa %}
    <li>

      {% assign date_format = site.cayman-blog.date_format | default: "%b %-d, %Y" %}
      <span class="post-meta">{{ post.date | date: date_format }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}" title="{{ post.title }}">{{ post.title | escape }}</a>
      </h2>

      <span>{{ post.excerpt | markdownify | truncatewords: 30 }}</span>

    </li>
  {% endfor %}
</ul>

<a href="/wiki/fa/">مشاهده بیشتر</a>

<hr>

<h3>English Wiki</h3>

<ul class="post-list">
  {% for post in site.wiki_en %}
    <li>

      {% assign date_format = site.cayman-blog.date_format | default: "%b %-d, %Y" %}
      <span class="post-meta">{{ post.date | date: date_format }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}" title="{{ post.title }}">{{ post.title | escape }}</a>
      </h2>

      <span>{{ post.excerpt | markdownify | truncatewords: 30 }}</span>

    </li>
  {% endfor %}
</ul>

<a href="/wiki/en/">Read more</a>
