---
layout: default
title: Writing
permalink: /blog/
---
<div class="container">
  <div class="page-hero">
    <h1 class="page-hero__title">Writing</h1>
    <p class="page-hero__sub">All essays, notes, and longer pieces — newest first.</p>
  </div>

  <ul class="post-list">
    {% for post in site.posts %}
    <li class="post-list__item">
      <time class="post-list__date" datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%b %-d, %Y" }}
      </time>
      <div>
        <a href="{{ post.url | relative_url }}">
          <h2 class="post-list__title">{{ post.title }}</h2>
        </a>
        <p class="post-list__excerpt">{{ post.excerpt | strip_html | truncatewords: 24 }}</p>
      </div>
    </li>
    {% endfor %}
  </ul>
</div>
