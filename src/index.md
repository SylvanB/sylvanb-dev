---
layout: default.liquid
---
## Posts

{% for post in collections.posts.pages %}
{% assign pubDateSplit = post.published_date | split: " " %}
{% assign pubDate = pubDateSplit[0] %}
**{{pubDate}}** - [{{ post.title }}]({{ post.permalink }})
{% endfor %}
