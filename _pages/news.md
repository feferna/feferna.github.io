---
title: "Recent Updates"
layout: single
permalink: /news/
---

{% assign news_items = site.news | sort: "date" | reverse %}
{% for item in news_items %}
  {% include archive-single.html %}
{% endfor %}