---
layout: default
title: blog
permalink: /blog_en/
description: Mundo Oceluna blog
lang: en
---

<ul class="post-list">
{% for post in site.posts %}
{% if post.lang == 'en' %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ post.description }}</p>
        <br/>
        <hr/>
      </li>
{% endif %}
{% endfor %}
