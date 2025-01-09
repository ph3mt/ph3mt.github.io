---
layout: archive
title: "Blog"
permalink: /blog/
entries_layout: grid
---

Welcome to the blog! Below, you’ll find all the posts organized by date.

<ul>
  {% for post in site.posts %}
    <li style="margin-bottom: 20px; list-style: none;">
      {% if post.featured_image %}
        <img src="{{ post.featured_image | relative_url }}" alt="Anteprima di {{ post.title }}" style="max-width: 150px; height: auto; margin-right: 10px; float: left; border-radius: 5px;">
      {% endif %}
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
      <div style="clear: both;"></div>
    </li>
  {% endfor %}
</ul>