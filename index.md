---
layout: blog
title: Litefy's Blog
---
{{page.title}}
=

{% for post in page.posts %}
*{{ post.date | date_to_string }} [post.title]({{site.baseurl}}{{post.url}})
{% endfor %}