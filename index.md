---
layout: default
title: Home
---

## Welcome

Bookmark this page to keep an eye on my projects, crazy ideas and nice things to read about virology, metal, sports and more.

[About me]({{ "/about.html" | relative_url }})

## Latest posts

{% for post in site.posts limit:10 %}
- {{ post.date | date: "%d %b %Y" }} – [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

{% if site.posts.size == 0 %}
Nothing here yet. Coming soon!
{% endif %}
