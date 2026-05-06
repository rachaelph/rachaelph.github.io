---
layout: page
permalink: /blog/
title: " "
---

<style>
  /* ===== Blog ===== */
  .bl { font-family: 'Georgia', 'Garamond', serif; color: #2c3e50; }

  .bl-hero {
    background: linear-gradient(135deg, rgba(44,95,111,0.82), rgba(13,138,154,0.7)),
                url('/assets/images/stpete.jpg') center/cover no-repeat;
    color: #fff;
    text-align: center;
    padding: 70px 24px 60px;
    border-radius: 14px;
    margin: 20px auto 30px;
    max-width: 1200px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.15);
  }
  .bl-hero h1 {
    color: #fff;
    font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive;
    font-size: 3.4em;
    margin: 0;
    letter-spacing: 2px;
    text-shadow: 0 2px 8px rgba(0,0,0,0.25);
  }
  .bl-hero p {
    font-style: italic;
    font-size: 1.2em;
    color: #fdf6ec;
    max-width: 700px;
    margin: 14px auto 0;
  }

  .bl-stats {
    max-width: 1100px;
    margin: 0 auto 20px;
    text-align: center;
    color: #2c5f6f;
    font-style: italic;
  }

  .blog-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    gap: 28px;
    max-width: 1200px;
    margin: 30px auto 50px;
    padding: 0 10px;
  }

  .blog-card {
    background: #fff;
    border-radius: 14px;
    overflow: hidden;
    box-shadow: 0 4px 16px rgba(0,0,0,0.08);
    transition: transform .25s ease, box-shadow .25s ease;
    display: flex;
    flex-direction: column;
  }
  .blog-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 12px 28px rgba(0,0,0,0.15);
  }

  .blog-card-image-wrap {
    position: relative;
    overflow: hidden;
    background: linear-gradient(135deg, #2c5f6f, #0d8a9a);
    aspect-ratio: 16 / 9;
  }
  .blog-card-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    transition: transform .4s ease;
  }
  .blog-card:hover .blog-card-image { transform: scale(1.04); }

  .blog-card-image-fallback {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
    color: #fdf6ec;
    font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive;
    font-size: 2.4em;
    text-align: center;
    padding: 20px;
  }

  .blog-card-content {
    padding: 22px 22px 24px;
    flex: 1;
    display: flex;
    flex-direction: column;
  }
  .blog-card-category {
    display: inline-block;
    background: #d4a574;
    color: #fff;
    padding: 4px 12px;
    border-radius: 20px;
    font-size: 0.78em;
    font-weight: bold;
    letter-spacing: 1px;
    margin-bottom: 12px;
    align-self: flex-start;
  }
  .blog-card-title {
    font-family: 'Georgia', serif;
    font-size: 1.4em;
    margin: 0 0 8px;
    color: #2c5f6f;
    line-height: 1.3;
  }
  .blog-card-title a {
    text-decoration: none;
    color: inherit;
    background-image: linear-gradient(currentColor, currentColor);
    background-size: 0% 1px;
    background-repeat: no-repeat;
    background-position: 0 100%;
    transition: background-size .25s ease;
  }
  .blog-card-title a:hover { background-size: 100% 1px; color: #0d8a9a; }
  .blog-card-meta { color: #888; font-size: 0.88em; margin-bottom: 10px; }
  .blog-card-excerpt { color: #555; line-height: 1.6; margin: 0; }
  .blog-card-readmore {
    margin-top: 14px;
    color: #d4a574;
    font-weight: bold;
    text-decoration: none;
    align-self: flex-start;
  }
  .blog-card-readmore:hover { color: #b8895a; }

  .bl-empty {
    max-width: 700px;
    margin: 60px auto;
    background: #fff;
    border-radius: 14px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.08);
    padding: 50px 30px;
    text-align: center;
    color: #666;
  }
  .bl-empty .icon { font-size: 3em; margin-bottom: 10px; }

  @media (max-width: 768px) {
    .bl-hero { padding: 50px 16px 45px; }
    .bl-hero h1 { font-size: 2.2em; }
    .bl-hero p { font-size: 1em; }
  }
</style>

{% include base_path %}

<div class="bl">

<section class="bl-hero">
  <h1>Adventures &amp; Stories</h1>
  <p>Travel, beach life, family gatherings, and everything in between — straight from the Sunshine City.</p>
</section>

{% if site.posts.size > 0 %}
<p class="bl-stats">{{ site.posts.size }} {% if site.posts.size == 1 %}story{% else %}stories{% endif %} and counting ✨</p>

<div class="blog-grid">
  {% for post in site.posts %}
    <article class="blog-card">
      <a href="{{ base_path }}{{ post.url }}" class="blog-card-image-wrap" aria-label="{{ post.title }}">
        {% if post.background_image %}
          <img src="{{ post.background_image }}" alt="{{ post.title }}" class="blog-card-image" loading="lazy">
        {% elsif post.feature_image %}
          <img src="{{ post.feature_image }}" alt="{{ post.title }}" class="blog-card-image" loading="lazy">
        {% else %}
          <div class="blog-card-image-fallback">{{ post.title | truncate: 40 }}</div>
        {% endif %}
      </a>
      <div class="blog-card-content">
        {% if post.categories[0] %}
        <span class="blog-card-category">{{ post.categories[0] | upcase }}</span>
        {% endif %}
        <h2 class="blog-card-title">
          <a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
        </h2>
        <p class="blog-card-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
        {% if post.excerpt %}
        <p class="blog-card-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
        {% endif %}
        <a href="{{ base_path }}{{ post.url }}" class="blog-card-readmore">Read more →</a>
      </div>
    </article>
  {% endfor %}
</div>
{% else %}
<div class="bl-empty">
  <div class="icon">✈️</div>
  <h2 style="color:#2c5f6f; margin-top:0;">No posts yet</h2>
  <p>Check back soon for our latest adventures!</p>
</div>
{% endif %}

</div>
