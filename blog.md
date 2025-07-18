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

