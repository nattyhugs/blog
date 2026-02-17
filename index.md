---
layout: default
---

# Recent Updates

{% for post in site.posts %}
## [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}
---
{% endfor %}

<link rel="stylesheet" href="{{ "/assets/css/style.css" | relative_url }}">
