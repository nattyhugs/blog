---
layout: default
---

# Recent Updates

{% for post in site.posts %}
### [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*
{% endfor %}

<style>
  body { background-color: #0d1117 !important; color: #c9d1d9 !important; }
  a { color: #58a6ff !important; }
  h1, h2, h3 { color: #58a6ff !important; }
</style>
