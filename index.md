---
layout: page
title: Litefy's Blog
---
{{page.title}}
=
{% for post in site.posts %}
* {{ post.date | date: "%Y-%m-%d" }} [{{post.title}}]({{site.baseurl}}{{post.url}})
{% endfor %}
