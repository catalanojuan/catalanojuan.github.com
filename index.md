---
layout: post
title: catalanojuan.github.com
subtitle: My Github hosted "blog like" stuff.
---
{% for post in site.posts %}
### {{ post.title }}

{{ post.description }} {% if post.type == 'proyect' %}[Code here.]({{post.repo_url}}){% else %}[More.]({{post.url}}){% endif %}
{% endfor %}
