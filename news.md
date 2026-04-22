---
layout: page
title: お知らせ
permalink: /news/
---

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
*{{ post.date | date: "%Y年%m月%d日" }}*
{{ post.excerpt | strip_html | truncatewords: 20 }}

---
{% endfor %}
