---
layout: default
---

<header class="site-header">
  <h1 class="site-title">Nate Hughes | Blog</h1>
  <p class="site-description">Distributed Systems & Agentic Explorer</p>
</header>

<main class="content">
  <section class="posts-list">
    <h2>Recent Updates</h2>
    <ul>
      {% for post in site.posts %}
        <li class="post-item">
          <span class="post-date">{{ post.date | date: "%b %d, %Y" }}</span>
          <a href="{{ site.baseurl }}{{ post.url }}" class="post-link">{{ post.title }}</a>
        </li>
      {% endfor %}
    </ul>
  </section>
</main>

<style>
  :root {
    --bg-color: #0d1117;
    --text-color: #c9d1d9;
    --accent-color: #58a6ff;
    --border-color: #30363d;
  }
  body {
    background-color: var(--bg-color);
    color: var(--text-color);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
    line-height: 1.6;
    max-width: 800px;
    margin: 0 auto;
    padding: 2rem;
  }
  .site-header {
    border-bottom: 1px solid var(--border-color);
    padding-bottom: 1rem;
    margin-bottom: 2rem;
  }
  .site-title { color: var(--accent-color); margin: 0; }
  .site-description { font-style: italic; opacity: 0.8; }
  h2 { border-bottom: 1px solid var(--border-color); padding-bottom: 0.5rem; }
  ul { list-style: none; padding: 0; }
  .post-item { margin-bottom: 1rem; display: flex; align-items: baseline; }
  .post-date { font-family: monospace; min-width: 120px; color: #8b949e; }
  .post-link { color: var(--accent-color); text-decoration: none; font-weight: bold; }
  .post-link:hover { text-decoration: underline; }
  a { color: var(--accent-color); }
</style>
