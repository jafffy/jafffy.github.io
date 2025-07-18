---
layout: page
title: Blog
permalink: /blog/
---

<div class="blog-posts">
  {% for post in site.posts %}
  <article class="blog-post-item">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <div class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
      {% if post.categories %}
      <span class="categories">
        in {% for category in post.categories %}{{ category }}{% unless forloop.last %}, {% endunless %}{% endfor %}
      </span>
      {% endif %}
    </div>
    <p class="excerpt">{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
    <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
  </article>
  {% endfor %}
</div>

<style>
.blog-posts {
  max-width: 800px;
  margin: 0 auto;
}

.blog-post-item {
  margin-bottom: 3rem;
  padding-bottom: 2rem;
  border-bottom: 1px solid #e5e7eb;
}

.blog-post-item:last-child {
  border-bottom: none;
}

.blog-post-item h2 {
  margin-bottom: 0.5rem;
}

.post-meta {
  color: #6b7280;
  font-size: 0.875rem;
  margin-bottom: 1rem;
}

.categories {
  margin-left: 0.5rem;
}

.excerpt {
  margin-bottom: 1rem;
  line-height: 1.7;
}

.read-more {
  font-weight: 500;
  color: #2563eb;
}

.read-more:hover {
  color: #1d4ed8;
}
</style>