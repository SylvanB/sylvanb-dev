---
layout: default.liquid
---

{% for post in collections.posts.pages %}
_{{post.published_date | date: "%D"}}_ [{{ post.title }}]({{ post.permalink }})
{% endfor %}
