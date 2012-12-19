---
layout: page
title: Litefy's Blog 偶然 自省 生活
---
{{ page.title }}
=
{% for post in site.posts %}
* {{ post.date | date: "%Y-%m-%d" }} [{{post.title}}]({{site.baseurl}}{{post.url}})
{% endfor %}
