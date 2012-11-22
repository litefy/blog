---
layout: page
title: Tag | Litefy's Blog
---
{{page.title}}
=
{% for tag in site.tags %} <button class="btn">[{{ tag[0] }}](#{{ tag[0] }})</button> {% endfor %}

{% for tag in site.tags %}
<div id="{{tag[0]}}">{{ tag[0] }}</div>
{% for post in tag[1] %}
{{post.date | date : "%Y-%m-%d"}}[{{post.title}}]({{site.baseurl}}/{{post.url}})
{% endfor %}
{% endfor %}
