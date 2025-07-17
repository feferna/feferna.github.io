---
layout: single
author_profile: true
---

{% comment %}
This is your homepage. You can customize the layout in _layouts/home.html.
{% endcomment %}

{% include base_path %}

{% assign about = site.pages | where: "permalink", "/about/" | first %}
{{ about.content }}

## 🔔 Recent Updates

{% assign news_posts = site.posts | where_exp: "post", "post.categories contains 'news'" %}
{% for post in news_posts limit: 5 %}
- **{{ post.date | date: "%b %-d, %Y" }}** — [{{ post.title }}]({{ post.url }})
{% endfor %}
