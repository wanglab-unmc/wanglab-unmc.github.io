---
title: News
nav:
  order: 6
  tooltip: Lab news
---

# {% include icon.html icon="fa-solid fa-newspaper" %}News
<ul>
{% for item in site.data.news.news %}
    <li>
        <strong>{{ item.date }}</strong> - {{ item.title }}
    </li>
{% endfor %}
</ul>
