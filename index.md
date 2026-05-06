---
title: " "
feature_image: "/assets/images/stpete.jpg"
excerpt: "Smith Family in the Sunshine City!"
---

<style>
  /* ===== Smith Seabreeze - Home ===== */
  .ss-home { font-family: 'Georgia', 'Garamond', serif; color: #2c3e50; }
  .ss-home h1, .ss-home h2, .ss-home h3 { font-family: 'Georgia', serif; color: #2c5f6f; }

  /* Hero */
  .ss-hero {
    position: relative;
    background: linear-gradient(135deg, rgba(44,95,111,0.85), rgba(13,138,154,0.75)),
                url('/assets/images/stpete.jpg') center/cover no-repeat;
    color: #fff;
    text-align: center;
    padding: 80px 20px 70px;
    border-radius: 14px;
    margin: 20px auto 40px;
    max-width: 1200px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.15);
  }
  .ss-hero h1 {
    color: #fff;
    font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive;
    font-size: 4em;
    margin: 0 0 8px;
    letter-spacing: 2px;
    text-shadow: 0 2px 8px rgba(0,0,0,0.25);
  }
  .ss-hero p.tag {
    font-size: 1.3em;
    font-style: italic;
    margin: 0 0 24px;
    color: #fdf6ec;
  }
  .ss-hero .pill {
    display: inline-block;
    background: #d4a574;
    color: #fff;
    padding: 10px 22px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    margin: 6px 6px 0;
    transition: transform .2s ease, box-shadow .2s ease;
  }
  .ss-hero .pill:hover { transform: translateY(-2px); box-shadow: 0 6px 14px rgba(0,0,0,0.2); }
  .ss-hero .pill.alt { background: rgba(255,255,255,0.15); border: 2px solid #fff; }

  /* Countdown */
  .ss-countdown {
    max-width: 900px;
    margin: -30px auto 40px;
    background: #fff;
    border-radius: 12px;
    padding: 20px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.08);
    text-align: center;
    position: relative;
    z-index: 2;
  }
  .ss-countdown .label {
    color: #d4a574;
    font-style: italic;
    letter-spacing: 1px;
    margin: 0 0 10px;
    font-size: 1em;
  }
  .ss-countdown .grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
    max-width: 520px;
    margin: 0 auto;
  }
  .ss-countdown .num {
    font-size: 2.2em;
    font-weight: bold;
    color: #2c5f6f;
    line-height: 1;
  }
  .ss-countdown .unit {
    font-size: 0.85em;
    color: #666;
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  /* Welcome card */
  .ss-welcome {
    max-width: 1100px;
    margin: 30px auto;
    background: #fff;
    border-radius: 14px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.08);
    padding: 40px;
    line-height: 1.7;
    font-size: 1.1em;
  }
  .ss-welcome h2 {
    text-align: center;
    border-bottom: 2px solid #d4a574;
    padding-bottom: 10px;
    margin-bottom: 20px;
    font-size: 2em;
  }

  /* Feature grid */
  .ss-features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 20px;
    max-width: 1100px;
    margin: 30px auto;
    padding: 0 10px;
  }
  .ss-feature {
    background: #fff;
    border-radius: 12px;
    padding: 25px 20px;
    text-align: center;
    box-shadow: 0 4px 14px rgba(0,0,0,0.07);
    border-top: 4px solid #d4a574;
    transition: transform .2s ease, box-shadow .2s ease;
  }
  .ss-feature:hover { transform: translateY(-4px); box-shadow: 0 10px 22px rgba(0,0,0,0.12); }
  .ss-feature .icon { font-size: 2.4em; margin-bottom: 10px; }
  .ss-feature h3 { margin: 0 0 8px; font-size: 1.2em; color: #2c5f6f; }
  .ss-feature p { margin: 0; color: #555; font-size: 0.95em; }

  /* Who we are */
  .ss-who {
    max-width: 1100px;
    margin: 40px auto;
    background: #fff;
    border-radius: 14px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.08);
    padding: 40px;
    display: grid;
    grid-template-columns: 1fr 320px;
    gap: 35px;
    align-items: center;
  }
  .ss-who img { width: 100%; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.15); }
  .ss-who h2 { margin-top: 0; border-bottom: 2px solid #d4a574; padding-bottom: 10px; font-size: 2em; }
  .ss-who p { line-height: 1.7; color: #444; font-size: 1.05em; }

  /* CTA */
  .ss-cta {
    max-width: 1100px;
    margin: 30px auto 50px;
    text-align: center;
    background: linear-gradient(135deg, #2c5f6f, #0d8a9a);
    color: #fff;
    padding: 40px 30px;
    border-radius: 14px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.12);
  }
  .ss-cta h2 { color: #fff; margin: 0 0 10px; font-size: 1.8em; }
  .ss-cta p { font-size: 1.1em; margin: 0 0 18px; color: #fdf6ec; }
  .ss-cta a {
    display: inline-block;
    background: #d4a574;
    color: #fff;
    padding: 12px 24px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    margin: 6px;
    transition: transform .2s ease, box-shadow .2s ease;
  }
  .ss-cta a:hover { transform: translateY(-2px); box-shadow: 0 6px 14px rgba(0,0,0,0.2); }

  @media (max-width: 768px) {
    .ss-hero { padding: 60px 16px 50px; }
    .ss-hero h1 { font-size: 2.6em; }
    .ss-hero p.tag { font-size: 1.05em; }
    .ss-welcome, .ss-who { padding: 24px; }
    .ss-who { grid-template-columns: 1fr; text-align: center; }
    .ss-countdown .num { font-size: 1.6em; }
  }
</style>

<div class="ss-home">

<section class="ss-hero">
  <h1>Smith Seabreeze</h1>
  <p class="tag">Smith Family in the Sunshine City ☀️🌊</p>
  <a class="pill" href="/about-us/">About Us</a>
  <a class="pill alt" href="/wedding/">Our Wedding 💍</a>
  <a class="pill alt" href="/blog/">The Blog</a>
</section>

<section class="ss-countdown" id="wedding-countdown">
  <p class="label">Counting down to <strong style="color:#2c5f6f;">April 15, 2027</strong></p>
  <div class="grid">
    <div><div class="num" id="cd-days">—</div><div class="unit">Days</div></div>
    <div><div class="num" id="cd-hours">—</div><div class="unit">Hours</div></div>
    <div><div class="num" id="cd-mins">—</div><div class="unit">Minutes</div></div>
    <div><div class="num" id="cd-secs">—</div><div class="unit">Seconds</div></div>
  </div>
</section>

<section class="ss-welcome">
  <h2>Welcome 👋</h2>
  <p>We're <strong>Rachael &amp; Jared</strong> — a family of beach lovers, adventure seekers, and dog parents living our best life in <strong>Saint Petersburg, Florida</strong>. This is our space to share our journey as we count down to our April 2027 wedding and everything in between!</p>
</section>

<section class="ss-features">
  <div class="ss-feature">
    <div class="icon">🌊</div>
    <h3>Beach Life</h3>
    <p>Living in the Sunshine City</p>
  </div>
  <div class="ss-feature">
    <div class="icon">✈️</div>
    <h3>Adventures</h3>
    <p>Travel stories &amp; weekend getaways</p>
  </div>
  <div class="ss-feature">
    <div class="icon">🐾</div>
    <h3>Ellie Updates</h3>
    <p>Our sweet 13-year-old pup</p>
  </div>
  <div class="ss-feature">
    <div class="icon">💍</div>
    <h3>Wedding Journey</h3>
    <p>Planning our 2027 celebration</p>
  </div>
  <div class="ss-feature">
    <div class="icon">🎯</div>
    <h3>Life &amp; Growth</h3>
    <p>Career, hobbies, and everything we love</p>
  </div>
</section>

<section class="ss-who">
  <div>
    <h2>Who We Are</h2>
    <p>A California girl and a Michigander who found each other in the Sunshine City! We're counting down to our April 2027 wedding while enjoying beach life with our 13-year-old pup, Ellie.</p>
    <p><strong>Rachael</strong> is a Senior Consultant in Data &amp; AI at Microsoft and loves pickleball, golf, and the Junior League of Saint Petersburg. <strong>Jared</strong> is a Product Sales Specialist for Adams Corporation and enjoys golf, pickleball, traveling, and weekend adventures.</p>
    <p>Together, we love traveling, volunteering, and making the most of our St. Pete life.</p>
    <p style="margin-top: 18px;"><a href="/about-us/" style="color:#d4a574; font-weight:bold; text-decoration:none;">Learn more about us →</a></p>
  </div>
  <img src="/assets/images/rachael-jared.jpg" alt="Rachael and Jared">
</section>

<section class="ss-cta">
  <h2>Follow Along</h2>
  <p>Read our latest stories, peek at the wedding plans, or get to know us a little better.</p>
  <a href="/blog/">📝 Read the Blog</a>
  <a href="/wedding/">💍 Wedding Details</a>
  <a href="/about-us/">💌 About Us</a>
</section>

</div>

<script>
  (function () {
    var target = new Date('2027-04-15T17:00:00-04:00').getTime();
    function tick() {
      var now = Date.now();
      var diff = Math.max(0, target - now);
      var d = Math.floor(diff / (1000 * 60 * 60 * 24));
      var h = Math.floor((diff / (1000 * 60 * 60)) % 24);
      var m = Math.floor((diff / (1000 * 60)) % 60);
      var s = Math.floor((diff / 1000) % 60);
      var elD = document.getElementById('cd-days');
      var elH = document.getElementById('cd-hours');
      var elM = document.getElementById('cd-mins');
      var elS = document.getElementById('cd-secs');
      if (elD) elD.textContent = d;
      if (elH) elH.textContent = h;
      if (elM) elM.textContent = m;
      if (elS) elS.textContent = s;
    }
    tick();
    setInterval(tick, 1000);
  })();
</script>
