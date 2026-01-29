---
layout: default
title: Home
---

# 👋 Hey, I'm Kejie

**Builder · Investor · AI Enthusiast**

欢迎来到我的个人空间。这里记录我的思考、投资笔记和技术探索。

---

## 📝 最新文章

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

{% if site.posts.size == 0 %}
*暂无文章，敬请期待...*
{% endif %}

---

## 🔗 Links

- [GitHub](https://github.com/kejie1024)
- [Blog](/blog)
- [About](/about)