---
layout: archive
title: "Blog"
permalink: /blog/
entries_layout: grid
---

Welcome to the blog! Below, you’ll find all the posts organized by date.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>