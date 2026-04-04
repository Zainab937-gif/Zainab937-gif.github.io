---
layout: default
title: Blog - Zainab Aamir
---

<div class="page-header">
  <h1>My Blog</h1>
  <p>Sharing my university journey, programming experiences, and technical learnings</p>
</div>

<div class="category-section">
  <h2>Programming Posts</h2>
  <div class="blog-grid">
    {% for post in site.programming %}
    <div class="blog-card">
      <span class="category-tag">Programming</span>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="date">{{ post.date | date: "%B %d, %Y" }}</p>
      <p>{{ post.excerpt | truncate: 100 }}</p>
    </div>
    {% endfor %}
  </div>
</div>

<div class="category-section">
  <h2>Database Posts</h2>
  <div class="blog-grid">
    {% for post in site.database %}
    <div class="blog-card">
      <span class="category-tag">Database</span>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="date">{{ post.date | date: "%B %d, %Y" }}</p>
      <p>{{ post.excerpt | truncate: 100 }}</p>
    </div>
    {% endfor %}
  </div>
</div>
