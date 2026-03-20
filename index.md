---
layout: default
---
<div class="container">
  <section class="home-hero">
    <p class="hero-kicker">A space for thinking</p>
    <h1 class="hero-headline">Writing that lingers<br><em>after the last line.</em></h1>
    <p class="hero-sub">Essays on craft, technology, and the quiet moments in between. Updated when something is worth saying.</p>
  </section>

  <section style="margin-bottom: 5rem;">
    <p class="section-label">Recent writing</p>
    <div class="post-grid">
      {% for post in site.posts limit:6 %}
      <a href="{{ post.url | relative_url }}" class="post-card">
        <p class="post-card__meta">{{ post.date | date: "%b %-d, %Y" }}{% if post.category %} · {{ post.category }}{% endif %}</p>
        <h2 class="post-card__title">{{ post.title }}</h2>
        <p class="post-card__excerpt">{{ post.excerpt | strip_html | truncatewords: 28 }}</p>
        <span class="post-card__link">Read more →</span>
      </a>
      {% endfor %}
    </div>
    <a href="{{ '/blog/' | relative_url }}" class="view-all">All posts</a>
  </section>
</div>
