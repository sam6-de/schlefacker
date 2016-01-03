---
layout: page
title: Blog
excerpt: "An archive of blog posts sorted by date."
search_omit: true
image:
  feature: blog.jpg
  credit: Skitter Photo
  creditlink: https://stocksnap.io/photo/CJSRRVR4JE
---

<ul class="post-list">
{% for post in site.categories.baublog %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
