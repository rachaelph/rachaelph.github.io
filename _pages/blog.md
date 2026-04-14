---
layout: page
permalink: /blog/
title: "Blog"
---

<style>
.blog-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
  gap: 30px;
  margin: 30px 0;
}

.blog-card {
  background: white;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.blog-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.15);
}

.blog-card-image {
  width: 100%;
  height: auto;
  aspect-ratio: 16 / 9;
  object-fit: cover;
  display: block;
}

.blog-card-content {
  padding: 20px;
}

.blog-card-title {
  font-size: 1.5em;
  margin: 0 0 10px 0;
  color: #2c5f6f;
}

.blog-card-title a {
  text-decoration: none;
  color: inherit;
}

.blog-card-title a:hover {
  color: #4a9fb8;
}

.blog-card-meta {
  color: #666;
  font-size: 0.9em;
  margin-bottom: 10px;
}

.blog-card-excerpt {
  color: #555;
  line-height: 1.6;
}

.blog-card-category {
  display: inline-block;
  background: #2c5f6f;
  color: white;
  padding: 5px 12px;
  border-radius: 5px;
  font-size: 0.85em;
  margin-bottom: 10px;
}
</style>

{% include base_path %}

{% if site.posts.size > 0 %}
<div class="blog-grid">
  {% for post in site.posts %}
    <div class="blog-card">
      {% if post.background_image %}
      <a href="{{ base_path }}{{ post.url }}">
        <img src="{{ post.background_image }}" alt="{{ post.title }}" class="blog-card-image">
      </a>
      {% endif %}
      <div class="blog-card-content">
        {% if post.categories[0] %}
        <span class="blog-card-category">{{ post.categories[0] | upcase }}</span>
        {% endif %}
        <h2 class="blog-card-title">
          <a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
        </h2>
        <p class="blog-card-meta">{{ post.date | date: "%B %Y" }}</p>
        {% if post.excerpt %}
        <p class="blog-card-excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>
{% else %}
  <p style="text-align: center; color: #999; font-style: italic; padding: 40px 0;">No posts yet — check back soon for our latest adventures! ✈️</p>
{% endif %}