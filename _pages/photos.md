---
layout: page
permalink: /photos/
title: " "
---

<style>
  /* ===== Photos / Albums ===== */
  .ph { font-family: 'Georgia', 'Garamond', serif; color: #2c3e50; }

  .ph-hero {
    background: linear-gradient(135deg, rgba(44,95,111,0.82), rgba(13,138,154,0.7)),
                url('/assets/images/stpete2.jpg') center/cover no-repeat;
    color: #fff;
    text-align: center;
    padding: 70px 24px 60px;
    border-radius: 14px;
    margin: 20px auto 30px;
    max-width: 1200px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.15);
  }
  .ph-hero h1 {
    color: #fff;
    font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive;
    font-size: 3.4em;
    margin: 0;
    letter-spacing: 2px;
    text-shadow: 0 2px 8px rgba(0,0,0,0.25);
  }
  .ph-hero p {
    font-style: italic;
    font-size: 1.2em;
    color: #fdf6ec;
    max-width: 700px;
    margin: 14px auto 0;
  }

  .ph-stats {
    max-width: 1100px;
    margin: 0 auto 20px;
    text-align: center;
    color: #2c5f6f;
    font-style: italic;
  }

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

  .ph-album-info {
    padding: 16px 18px 20px;
  }
  .ph-album-title {
    color: #2c5f6f;
    font-size: 1.2em;
    margin: 0 0 4px;
    font-family: 'Georgia', serif;
  }
  .ph-album-date { color: #888; font-size: 0.9em; margin: 0; font-style: italic; }

  /* Album panel (expanded view) */
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
    .ph-hero { padding: 50px 16px 45px; }
    .ph-hero h1 { font-size: 2.2em; }
    .ph-thumbs { grid-template-columns: repeat(auto-fill, minmax(120px, 1fr)); }
    .ph-lb-btn { width: 40px; height: 40px; font-size: 1.2em; }
    .ph-lb-prev { left: 8px; }
    .ph-lb-next { right: 8px; }
  }
</style>

<div class="ph">

<section class="ph-hero">
  <h1>Photos</h1>
  <p>Adventures, family, friends, and everyday moments — captured along the way.</p>
</section>

{% assign sorted_albums = site.data.photos.albums | sort: "date" | reverse %}

<p class="ph-stats">{{ sorted_albums | size }} albums &middot; click any cover to view photos</p>

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
