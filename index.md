---
layout: default
---

# Nate Hughes | Blog

Welcome to my personal feed. Here I document my work in distributed systems, AI agents, and more.

## Posts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>
