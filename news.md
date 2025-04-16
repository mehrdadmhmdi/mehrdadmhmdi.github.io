---
layout: page
title: "News Archive"
permalink: /news/
---

<h1>News Archive</h1>
<ul>
  {% assign all_news = site.news | sort: 'date' | reverse %}
  {% for item in all_news %}
    <li>
      <strong>{{ item.date | date: "%B %d, %Y" }}:</strong>
      <a href="{{ item.url }}">{{ item.title }}</a>
    </li>
  {% endfor %}
</ul>
