---
layout: default
---

<div class="site-header">
  <h1 class="site-title">Nate Hughes | Blog</h1>
  <p class="site-description">Distributed Systems & Agentic Explorer</p>
</div>

<div class="content">
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
</div>

<style>
  /* Use !important to override the theme defaults aggressively */
  :root {
    --bg-color: #0d1117 !important;
    --text-color: #c9d1d9 !important;
    --accent-color: #58a6ff !important;
    --border-color: #30363d !important;
  }
  
  html, body, .container-lg, .site-header, .main-content, .footer {
    background-color: #0d1117 !important;
    color: #c9d1d9 !important;
  }

  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
    line-height: 1.6;
    max-width: 800px;
    margin: 0 auto;
    padding: 2rem;
  }

  h1, h2, h3, h4, h5, h6 { color: #58a6ff !important; }
  
  .site-header {
    border-bottom: 1px solid #30363d !important;
    padding-bottom: 1rem;
    margin-bottom: 2rem;
  }
  
  .site-title { color: #58a6ff !important; margin: 0; }
  .site-description { font-style: italic; opacity: 0.8; }
  
  h2 { border-bottom: 1px solid #30363d !important; padding-bottom: 0.5rem; }
  
  ul { list-style: none; padding: 0; }
  
  .post-item { 
    margin-bottom: 1rem; 
    display: flex; 
    align-items: baseline; 
    border-bottom: 1px solid #21262d;
    padding-bottom: 0.5rem;
  }
  
  .post-date { 
    font-family: monospace; 
    min-width: 120px; 
    color: #8b949e !important; 
  }
  
  .post-link { 
    color: #58a6ff !important; 
    text-decoration: none; 
    font-weight: bold; 
  }
  
  .post-link:hover { text-decoration: underline; }
  
  a { color: #58a6ff !important; }
  
  code { background-color: #161b22 !important; color: #e6edf3 !important; padding: 0.2rem 0.4rem; border-radius: 6px; }
</style>
