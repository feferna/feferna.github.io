---
title: "Recent Updates"
layout: collection
collection: news
permalink: /news/
entries_layout: list
---

{% assign news_items = site.news | sort: "date" | reverse %}
{% for item in news_items %}
  {% include archive-single.html %}
{% endfor %}
