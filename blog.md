---
layout: default
title: Blog
permalink: /blog/
---

# 📚 Blog

所有文章列表：

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
{{ post.date | date: "%Y-%m-%d" }} · {{ post.categories | join: ", " }}

{{ post.excerpt | strip_html | truncate: 150 }}

---
{% endfor %}

{% if site.posts.size == 0 %}
*暂无文章，敬请期待...*
{% endif %}