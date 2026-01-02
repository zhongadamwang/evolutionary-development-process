---
layout: page
title: Chapters
permalink: /chapters/
---

<ul>
{% assign sorted = site.chapters | sort: "order" %}
{% for chapter in sorted %}
  <li><a href="{{ chapter.url | relative_url }}">{{ chapter.title }}</a></li>
{% endfor %}
</ul>
