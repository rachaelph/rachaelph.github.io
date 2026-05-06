---
layout: page
permalink: /adventures/
title: " "
---

<style>
  /* ===== Adventures (Stories + Albums) ===== */
  .adv { font-family: 'Georgia', 'Garamond', serif; color: #2c3e50; }

  .adv-hero {
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
  .adv-hero h1 {
    color: #fff;
    font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive;
    font-size: 3.4em;
    margin: 0;
    letter-spacing: 2px;
    text-shadow: 0 2px 8px rgba(0,0,0,0.25);
  }
  .adv-hero p {
    font-style: italic;
    font-size: 1.2em;
    color: #fdf6ec;
    max-width: 700px;
    margin: 14px auto 0;
  }

  /* Tab switcher */
  .adv-tabs {
    max-width: 1200px;
    margin: 0 auto 20px;
    display: flex;
    justify-content: center;
    gap: 10px;
    flex-wrap: wrap;
    padding: 0 10px;
  }
  .adv-tab {
    background: #fff;
    color: #2c5f6f;
    border: 2px solid #2c5f6f;
    padding: 10px 26px;
    border-radius: 24px;
    font-family: 'Georgia', serif;
    font-size: 1em;
    font-weight: bold;
    cursor: pointer;
    transition: all .2s ease;
  }
  .adv-tab:hover { background: #fdf6ec; }
  .adv-tab.is-active {
    background: #2c5f6f;
    color: #fff;
  }

  .adv-pane { display: none; }
  .adv-pane.is-active { display: block; }

  .adv-stats {
    max-width: 1100px;
    margin: 0 auto 20px;
    text-align: center;
    color: #2c5f6f;
    font-style: italic;
  }

  /* ---- Stories grid (formerly blog) ---- */
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
    width: 100%; height: 100%; object-fit: cover; display: block;
    transition: transform .4s ease;
  }
  .blog-card:hover .blog-card-image { transform: scale(1.04); }
  .blog-card-image-fallback {
    display: flex; align-items: center; justify-content: center;
    height: 100%; color: #fdf6ec;
    font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive;
    font-size: 2.4em; text-align: center; padding: 20px;
  }
  .blog-card-content {
    padding: 22px 22px 24px;
    flex: 1; display: flex; flex-direction: column;
  }
  .blog-card-category {
    display: inline-block;
    background: #d4a574; color: #fff;
    padding: 4px 12px; border-radius: 20px;
    font-size: 0.78em; font-weight: bold;
    letter-spacing: 1px; margin-bottom: 12px;
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
    margin-top: 14px; color: #d4a574;
    font-weight: bold; text-decoration: none;
    align-self: flex-start;
  }
  .blog-card-readmore:hover { color: #b8895a; }
  .adv-empty {
    max-width: 700px;
    margin: 60px auto;
    background: #fff;
    border-radius: 14px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.08);
    padding: 50px 30px;
    text-align: center;
    color: #666;
  }
  .adv-empty .icon { font-size: 3em; margin-bottom: 10px; }

  /* ---- Albums (formerly photos) ---- */
  .ph-albums {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 24px;
    max-width: 1200px;
    margin: 30px auto 50px;
    padding: 0 10px;
  }
  .ph-album {
    background: #fff;
    border-radius: 14px;
    overflow: hidden;
    box-shadow: 0 4px 16px rgba(0,0,0,0.08);
    cursor: pointer;
    transition: transform .25s ease, box-shadow .25s ease;
    border: none;
    text-align: left;
    padding: 0;
    font: inherit;
    color: inherit;
    width: 100%;
    display: block;
  }
  .ph-album:hover {
    transform: translateY(-6px);
    box-shadow: 0 12px 28px rgba(0,0,0,0.15);
  }
  .ph-album-cover {
    position: relative;
    aspect-ratio: 4 / 3;
    overflow: hidden;
    background: linear-gradient(135deg, #2c5f6f, #0d8a9a);
  }
  .ph-album-cover img {
    width: 100%; height: 100%; object-fit: cover; display: block;
    transition: transform .4s ease;
  }
  .ph-album:hover .ph-album-cover img { transform: scale(1.05); }
  .ph-album-cover .count {
    position: absolute; bottom: 10px; right: 10px;
    background: rgba(0,0,0,0.55); color: #fff;
    padding: 4px 10px; border-radius: 14px;
    font-size: 0.8em; letter-spacing: 0.5px;
  }
  .ph-album-info { padding: 16px 18px 20px; }
  .ph-album-title {
    color: #2c5f6f;
    font-size: 1.2em;
    margin: 0 0 4px;
    font-family: 'Georgia', serif;
  }
  .ph-album-date { color: #888; font-size: 0.9em; margin: 0; font-style: italic; }

  .ph-album-panel {
    display: none;
    max-width: 1200px;
    margin: 30px auto;
    background: #fff;
    border-radius: 14px;
    padding: 26px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.08);
  }
  .ph-album-panel.is-open { display: block; }
  .ph-album-panel header {
    display: flex; align-items: center; justify-content: space-between;
    flex-wrap: wrap; gap: 12px; margin-bottom: 18px;
    border-bottom: 2px solid #d4a574; padding-bottom: 12px;
  }
  .ph-album-panel h2 {
    margin: 0; color: #2c5f6f; font-family: 'Georgia', serif; font-size: 1.6em;
  }
  .ph-album-panel .close {
    background: #d4a574; color: #fff; border: none;
    padding: 8px 16px; border-radius: 20px; font-weight: bold;
    cursor: pointer; font-size: 0.9em;
  }
  .ph-album-panel .close:hover { background: #b8895a; }

  .ph-thumbs {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
    gap: 10px;
  }
  .ph-thumb {
    aspect-ratio: 1 / 1;
    overflow: hidden;
    border-radius: 8px;
    cursor: pointer;
    background: #eee;
  }
  .ph-thumb img {
    width: 100%; height: 100%; object-fit: cover; display: block;
    transition: transform .3s ease;
  }
  .ph-thumb:hover img { transform: scale(1.08); }

  /* Lightbox */
  .ph-lightbox {
    position: fixed; inset: 0;
    background: rgba(0,0,0,0.92);
    display: none;
    align-items: center; justify-content: center;
    z-index: 9999;
    padding: 20px;
  }
  .ph-lightbox.is-open { display: flex; }
  .ph-lightbox img {
    max-width: 95vw; max-height: 88vh;
    border-radius: 8px; box-shadow: 0 10px 30px rgba(0,0,0,0.5);
  }
  .ph-lb-btn {
    position: absolute;
    background: rgba(255,255,255,0.15);
    border: 2px solid rgba(255,255,255,0.4);
    color: #fff;
    width: 48px; height: 48px;
    border-radius: 50%;
    font-size: 1.5em;
    cursor: pointer;
    display: flex; align-items: center; justify-content: center;
    transition: background .2s ease;
  }
  .ph-lb-btn:hover { background: rgba(255,255,255,0.3); }
  .ph-lb-prev { left: 20px; top: 50%; transform: translateY(-50%); }
  .ph-lb-next { right: 20px; top: 50%; transform: translateY(-50%); }
  .ph-lb-close { top: 20px; right: 20px; }
  .ph-lb-counter {
    position: absolute; bottom: 20px; left: 50%; transform: translateX(-50%);
    color: #fff; font-size: 0.95em; opacity: 0.8;
  }

  @media (max-width: 768px) {
    .adv-hero { padding: 50px 16px 45px; }
    .adv-hero h1 { font-size: 2.2em; }
    .adv-hero p { font-size: 1em; }
    .adv-tab { padding: 8px 18px; font-size: 0.95em; }
    .ph-thumbs { grid-template-columns: repeat(auto-fill, minmax(120px, 1fr)); }
    .ph-lb-btn { width: 40px; height: 40px; font-size: 1.2em; }
    .ph-lb-prev { left: 8px; }
    .ph-lb-next { right: 8px; }
  }
</style>

{% include base_path %}

<div class="adv">

<section class="adv-hero">
  <h1>Adventures</h1>
  <p>Stories, photos, and snapshots from our travels, family time, and life in the Sunshine City.</p>
</section>

<div class="adv-tabs" role="tablist">
  <button type="button" class="adv-tab is-active" role="tab" aria-selected="true" data-pane="stories">📝 Stories</button>
  <button type="button" class="adv-tab" role="tab" aria-selected="false" data-pane="albums">📸 Photo Albums</button>
</div>

<!-- ============== STORIES PANE ============== -->
<div class="adv-pane is-active" id="pane-stories" role="tabpanel">
  {% if site.posts.size > 0 %}
  <p class="adv-stats">{{ site.posts.size }} {% if site.posts.size == 1 %}story{% else %}stories{% endif %} and counting ✨</p>
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
  <div class="adv-empty">
    <div class="icon">✈️</div>
    <h2 style="color:#2c5f6f; margin-top:0;">No stories yet</h2>
    <p>Check back soon for our latest adventures!</p>
  </div>
  {% endif %}
</div>

<!-- ============== ALBUMS PANE ============== -->
<div class="adv-pane" id="pane-albums" role="tabpanel">
  {% assign sorted_albums = site.data.photos.albums | sort: "date" | reverse %}
  <p class="adv-stats">{{ sorted_albums | size }} albums &middot; click any cover to view photos</p>

  <div class="ph-albums">
    {% for album in sorted_albums %}
    <button type="button" class="ph-album" data-album="{{ forloop.index0 }}">
      <div class="ph-album-cover">
        <img src="/assets/images/{{ album.folder }}/{{ album.cover | uri_escape }}" alt="{{ album.title }}" loading="lazy">
        <span class="count">{{ album.photos | size }} photos</span>
      </div>
      <div class="ph-album-info">
        <h3 class="ph-album-title">{{ album.title }}</h3>
        <p class="ph-album-date">{{ album.date | date: "%B %Y" }}</p>
      </div>
    </button>
    {% endfor %}
  </div>

  {% for album in sorted_albums %}
  <section class="ph-album-panel" id="album-{{ forloop.index0 }}" data-album-folder="{{ album.folder }}">
    <header>
      <div>
        <h2>{{ album.title }}</h2>
        <p class="ph-album-date" style="margin: 4px 0 0;">{{ album.date | date: "%B %Y" }} &middot; {{ album.photos | size }} photos</p>
      </div>
      <button type="button" class="close" data-close>Close ✕</button>
    </header>
    <div class="ph-thumbs">
      {% for photo in album.photos %}
      <div class="ph-thumb" data-index="{{ forloop.index0 }}" data-src="/assets/images/{{ album.folder }}/{{ photo | uri_escape }}">
        <img src="/assets/images/{{ album.folder }}/{{ photo | uri_escape }}" alt="{{ album.title }} photo {{ forloop.index }}" loading="lazy">
      </div>
      {% endfor %}
    </div>
  </section>
  {% endfor %}
</div>

</div>

<!-- Lightbox -->
<div class="ph-lightbox" id="ph-lightbox" role="dialog" aria-modal="true" aria-label="Photo viewer">
  <button type="button" class="ph-lb-btn ph-lb-close" id="ph-lb-close" aria-label="Close">✕</button>
  <button type="button" class="ph-lb-btn ph-lb-prev" id="ph-lb-prev" aria-label="Previous photo">‹</button>
  <img id="ph-lb-img" src="" alt="">
  <button type="button" class="ph-lb-btn ph-lb-next" id="ph-lb-next" aria-label="Next photo">›</button>
  <div class="ph-lb-counter" id="ph-lb-counter"></div>
</div>

<script>
(function () {
  // ---- Tab switcher ----
  var tabs = document.querySelectorAll('.adv-tab');
  var panes = document.querySelectorAll('.adv-pane');
  function activate(name) {
    tabs.forEach(function (t) {
      var on = t.getAttribute('data-pane') === name;
      t.classList.toggle('is-active', on);
      t.setAttribute('aria-selected', on ? 'true' : 'false');
    });
    panes.forEach(function (p) {
      p.classList.toggle('is-active', p.id === 'pane-' + name);
    });
  }
  tabs.forEach(function (t) {
    t.addEventListener('click', function () {
      activate(t.getAttribute('data-pane'));
      // update hash for shareable links
      history.replaceState(null, '', '#' + t.getAttribute('data-pane'));
    });
  });
  // Honor hash on load (#stories or #albums)
  var initial = (location.hash || '').replace('#', '');
  if (initial === 'albums' || initial === 'stories') activate(initial);

  // ---- Album expand + lightbox ----
  var albums = document.querySelectorAll('.ph-album');
  var panels = document.querySelectorAll('.ph-album-panel');
  var lightbox = document.getElementById('ph-lightbox');
  var lbImg = document.getElementById('ph-lb-img');
  var lbCounter = document.getElementById('ph-lb-counter');
  var lbClose = document.getElementById('ph-lb-close');
  var lbPrev = document.getElementById('ph-lb-prev');
  var lbNext = document.getElementById('ph-lb-next');
  var currentPhotos = [];
  var currentIndex = 0;

  function closeAllPanels() {
    panels.forEach(function (p) { p.classList.remove('is-open'); });
  }
  albums.forEach(function (btn) {
    btn.addEventListener('click', function () {
      var idx = btn.getAttribute('data-album');
      closeAllPanels();
      var panel = document.getElementById('album-' + idx);
      if (panel) {
        panel.classList.add('is-open');
        panel.scrollIntoView({ behavior: 'smooth', block: 'start' });
      }
    });
  });
  panels.forEach(function (panel) {
    var closeBtn = panel.querySelector('[data-close]');
    if (closeBtn) {
      closeBtn.addEventListener('click', function () {
        panel.classList.remove('is-open');
        document.querySelector('.ph-albums').scrollIntoView({ behavior: 'smooth' });
      });
    }
    var thumbs = panel.querySelectorAll('.ph-thumb');
    var photos = Array.prototype.map.call(thumbs, function (t) { return t.getAttribute('data-src'); });
    thumbs.forEach(function (t, i) {
      t.addEventListener('click', function () {
        currentPhotos = photos;
        currentIndex = i;
        showLightbox();
      });
    });
  });

  function showLightbox() {
    lbImg.src = currentPhotos[currentIndex];
    lbImg.alt = 'Photo ' + (currentIndex + 1) + ' of ' + currentPhotos.length;
    lbCounter.textContent = (currentIndex + 1) + ' / ' + currentPhotos.length;
    lightbox.classList.add('is-open');
    document.body.style.overflow = 'hidden';
  }
  function hideLightbox() {
    lightbox.classList.remove('is-open');
    document.body.style.overflow = '';
  }
  function next() {
    if (!currentPhotos.length) return;
    currentIndex = (currentIndex + 1) % currentPhotos.length;
    showLightbox();
  }
  function prev() {
    if (!currentPhotos.length) return;
    currentIndex = (currentIndex - 1 + currentPhotos.length) % currentPhotos.length;
    showLightbox();
  }
  lbClose.addEventListener('click', hideLightbox);
  lbNext.addEventListener('click', next);
  lbPrev.addEventListener('click', prev);
  lightbox.addEventListener('click', function (e) {
    if (e.target === lightbox) hideLightbox();
  });
  document.addEventListener('keydown', function (e) {
    if (!lightbox.classList.contains('is-open')) return;
    if (e.key === 'Escape') hideLightbox();
    else if (e.key === 'ArrowRight') next();
    else if (e.key === 'ArrowLeft') prev();
  });
})();
</script>
