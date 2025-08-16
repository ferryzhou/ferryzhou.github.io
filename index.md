---
layout: home
title: "ferryzhou"
subtitle: "fragments of thoughts and time."
---

<div class="posts">
  {% for post in site.posts limit:50 %}
    <article class="post">
      <h2 class="post-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h2>
      
      <div class="post-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">
          {{ post.date | date: "%B %d, %Y" }}
        </time>
      </div>
      
      <div class="post-content">
        {% if post.excerpt %}
          {{ post.excerpt }}
        {% else %}
          {{ post.content | strip_html | truncatewords: 200 }}
        {% endif %}
      </div>
      
      <div class="post-footer">
        <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
      </div>
    </article>
    
    {% unless forloop.last %}
      <hr class="post-divider">
    {% endunless %}
  {% endfor %}
</div>

<div class="view-all-posts">
  <a href="{{ '/archive' | relative_url }}" class="view-all-link">View all posts →</a>
</div>
