---
layout: blog
title: Litefy's Blog
---
{{page.title}}
=

page.posts
{% for post in page.posts %}
*{{ post.date | date_to_string }} [post.title]({{site.baseurl}}{{post.url}})
{% endfor %}