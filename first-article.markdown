---
title: first article
date: 2016-11-26 04:14:00 Z
author: author1
---

where is this displayed?????

{% assign author = site.authors | where: 'title', post.author | first %}
{% if author %}
  <a href="{{ author.url }}">{{ author.title }}</a>
{% endif %}