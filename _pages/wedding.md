---
layout: page
permalink: /wedding/
---

<style>
  /* Elegant wedding page styling */

  html { scroll-behavior: smooth; }

  /* Sandy background for entire page */
  body {
    background-color: #F6F1E8 !important;
  }

  /* Countdown widget */
  .wed-countdown {
    max-width: 1000px;
    margin: 30px auto;
    background: #fff;
    border-radius: 12px;
    padding: 22px 20px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.10);
    text-align: center;
  }
  .wed-countdown .label {
    color: #d4a574;
    font-style: italic;
    letter-spacing: 1px;
    margin: 0 0 12px;
  }
  .wed-countdown .grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
    max-width: 540px;
    margin: 0 auto;
  }
  .wed-countdown .num {
    font-size: 2.2em;
    font-weight: bold;
    color: #2c5f6f;
    line-height: 1;
    font-family: 'Georgia', serif;
  }
  .wed-countdown .unit {
    font-size: 0.85em;
    color: #666;
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  @media (max-width: 480px) {
    .wed-countdown .num { font-size: 1.6em; }
  }
  
  /* Override theme width constraints */
  .page__content,
  .page-content,
  article,
  main {
    max-width: 100% !important;
    margin-left: auto !important;
    margin-right: auto !important;
    background-color: #F6F1E8;
  }
  
  .wedding-page {
    font-family: 'Georgia', 'Garamond', serif;
    background-color: #F6F1E8;
  }
  
  .wedding-title {
    text-align: center;
    margin: 40px 0;
    font-family: 'Georgia', serif;
  }
  
  .wedding-title h1 {
    color: #d4a574;
    font-size: 3em;
    margin-bottom: 10px;
    font-weight: normal;
    letter-spacing: 2px;
  }
  
  .wedding-title h2 {
    color: #2c5f6f;
    font-size: 1.8em;
    font-weight: 300;
    margin: 5px 0;
  }
  
  .wedding-title p {
    color: #666;
    font-size: 1.2em;
    font-style: italic;
  }
  
  .wedding-section {
    background: rgba(255, 255, 255, 0.9);
    padding: 10px;
    margin: 30px auto;
    max-width: 1200px;
    border-radius: 0;
    box-shadow: 0 4px 15px rgba(0,0,0,0.1);
  }
  
  .wedding-section h2 {
    color: #2c5f6f;
    font-size: 2em;
    border-bottom: 2px solid #d4a574;
    padding-bottom: 10px;
    margin-bottom: 20px;
    font-family: 'Georgia', serif;
  }
  
  .wedding-section h3 {
    color: #2c5f6f;
    font-size: 1.5em;
    margin-top: 25px;
    font-family: 'Georgia', serif;
  }
  
  .our-wedding-title {
    text-align: center;
    margin: 40px 0 20px 0;
  }
  
  .our-wedding-title h1 {
    font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive;
    font-size: 4em;
    color: #0d8a9a;
    margin: 0;
    font-weight: 400;
    letter-spacing: 2px;
  }
  
  .couple-photo {
    text-align: center;
    margin: 30px auto 40px auto;
  }
  
  .couple-photo img {
    max-width: 500px;
    width: 100%;
    border-radius: 15px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.2);
  }
  
  /* Mobile Responsive Styles */
  @media screen and (max-width: 768px) {
    /* Scale down all font sizes for tablets */
    .wedding-title h1 {
      font-size: 2em !important;
    }
    
    .wedding-title h2 {
      font-size: 1.3em !important;
    }
    
    .wedding-title p {
      font-size: 1em !important;
    }
    
    .our-wedding-title h1 {
      font-size: 2.5em !important;
    }
    
    .wedding-section h2 {
      font-size: 1.6em !important;
    }
    
    .wedding-section h3 {
      font-size: 1.3em !important;
    }
    
    .wedding-section h4 {
      font-size: 1.1em !important;
    }
    
    /* Reduce padding for sections */
    .wedding-section {
      padding: 15px !important;
      margin: 20px auto !important;
    }
    
    /* Make wedding party images smaller on tablets */
    img[alt*="Parsons"],
    img[alt*="Smith"],
    img[alt*="Ocasion"],
    img[alt*="Breneisen"],
    img[alt*="Berlinghoff"],
    img[alt*="Du"],
    img[alt*="Shemka"],
    img[alt*="Clark"],
    img[alt*="Copenhagen"],
    img[alt*="Howard"],
    img[alt*="Arellano"] {
      width: 200px !important;
      height: 200px !important;
    }
    
    /* Center header content on smaller screens */
    .our-wedding-title {
      text-align: center !important;
    }
    
    .wedding-title {
      text-align: center !important;
    }
    
    /* Reduce padding in payment section */
    div[style*="background: #f5f5f5"] {
      padding: 20px 10px !important;
    }
  }
  
  @media screen and (max-width: 480px) {
    /* Further scaling for phones */
    .wedding-title h1 {
      font-size: 1.5em !important;
      letter-spacing: 1px !important;
    }
    
    .wedding-title h2 {
      font-size: 1.1em !important;
    }
    
    .wedding-title p {
      font-size: 0.95em !important;
    }
    
    .our-wedding-title h1 {
      font-size: 2em !important;
      letter-spacing: 1px !important;
    }
    
    .wedding-section {
      padding: 10px !important;
      margin: 15px 5px !important;
    }
    
    .wedding-section h2 {
      font-size: 1.4em !important;
    }
    
    .wedding-section h3 {
      font-size: 1.15em !important;
    }
    
    .wedding-section h4 {
      font-size: 1em !important;
    }
    
    .wedding-page {
      padding: 10px 0 !important;
    }
    
    /* Make wedding party images even smaller on phones and stack text */
    img[alt*="Parsons"],
    img[alt*="Smith"],
    img[alt*="Ocasion"],
    img[alt*="Breneisen"],
    img[alt*="Berlinghoff"],
    img[alt*="Du"],
    img[alt*="Shemka"],
    img[alt*="Clark"],
    img[alt*="Copenhagen"],
    img[alt*="Howard"],
    img[alt*="Arellano"] {
      width: 150px !important;
      height: 150px !important;
    }
    
    /* Further reduce payment section padding on phones */
    div[style*="background: #f5f5f5"] {
      padding: 15px 5px !important;
      margin: 20px 0 !important;
    }
  }
</style>

<div class="wedding-page" id="top" style="padding: 20px 0;">

<div style="display: flex; gap: 40px; align-items: center; margin: 40px auto; max-width: 1200px; padding: 0 20px; flex-wrap: wrap;">
  
  <div style="flex: 1; min-width: 280px;">
    <div class="our-wedding-title" style="text-align: left; margin: 0 0 20px 0;">
      <h1 style="font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive; font-size: 3em; color: #0d8a9a; margin: 0; font-weight: 400; letter-spacing: 2px;">Our Wedding</h1>
    </div>
    
    <div class="wedding-title" style="text-align: left;">
      <h1 style="color: #00695C; font-size: 1.8em; margin-bottom: 10px; font-weight: normal; letter-spacing: 2px;"> Jared & Rachael </h1>
      <h2 style="color: #2c5f6f; font-size: 1.5em; font-weight: 300; margin: 5px 0;"> April 15, 2027 </h2>
      <p style="color: #666; font-size: 1.2em; font-style: italic;"> Madeira Beach, Florida </p>
    </div>
  </div>
  
  <div style="flex: 0 0 350px; min-width: 280px; max-width: 100%;">
    <img loading="lazy" src="/assets/images/wedding_logo.png" alt="Rachael & Jared Wedding Logo" style="max-width: 100%; width: 100%; height: auto;">
  </div>
  
</div>

<!-- Engagement Photo -->
<div style="text-align: center; margin: 40px auto;">
  <img loading="lazy" src="/assets/images/engagementphotos8.jpeg" alt="Rachael and Jared" style="max-width: 600px; width: 100%; border-radius: 15px; box-shadow: 0 6px 20px rgba(0,0,0,0.2);">
</div>

<!-- Wedding Countdown -->
<div class="wed-countdown">
  <p class="label">Counting down to <strong style="color:#2c5f6f;">April 15, 2027</strong> 🌴</p>
  <div class="grid">
    <div><div class="num" id="wcd-days">—</div><div class="unit">Days</div></div>
    <div><div class="num" id="wcd-hours">—</div><div class="unit">Hours</div></div>
    <div><div class="num" id="wcd-mins">—</div><div class="unit">Minutes</div></div>
    <div><div class="num" id="wcd-secs">—</div><div class="unit">Seconds</div></div>
  </div>
</div>

<!-- Quick Links Navigation -->
<div style="background: rgba(255, 255, 255, 0.95); padding: 20px; margin: 30px auto; text-align: center; box-shadow: 0 4px 15px rgba(0,0,0,0.1); max-width: 1000px; border-radius: 10px;">
  <p style="color: #2c5f6f; font-weight: bold; margin-bottom: 15px; font-size: 1.1em;">Quick Links</p>
  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; padding: 0 10px;">
    <a href="#event-details" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Venue & Schedule</a>
    <a href="#wedding-party" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Wedding Party</a>
    <a href="#travel-info" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Travel & Activities</a>
    <a href="https://www.honeyfund.com/site/phillips-weber-smith-04-15-2027?no_gdpr=1" target="_blank" rel="noopener" style="background: #d4a574; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Honeymoon Fund 🌴</a>
    <a href="#rsvp" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">RSVP</a>
    <a href="#faqs" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">FAQs</a>
  </div>
</div>

<div class="wedding-section" id="event-details">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Venue & Schedule</h2>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Event Details</h3>

<p><strong>📅 Date:</strong> Thursday, April 15, 2027<br>
<strong>🕐 Ceremony:</strong> 5:00 PM<br>
<strong>📍 Ceremony Address:</strong> Gulf Blvd & 134th Ave West (Beach Wedding)<br>
<strong>📍 Reception Venue:</strong> <a href="https://www.thewesteventspace.com/" target="_blank">The West Events</a><br>
<strong>🏠 Reception Address:</strong> 13435 Gulf Boulevard, Madeira Beach, FL 33708<br>
<strong>📞 Phone:</strong> (727) 363-4255</p>

<div style="background: #e8f4f8; padding: 20px; margin: 20px 0; border-left: 4px solid #2c5f6f; border-radius: 5px;">
  <p style="margin: 0;"><strong>🏖️ Beach Ceremony Information:</strong></p>
  <p style="margin: 10px 0 0 0;">Our ceremony will take place right on the beach! Please note:</p>
  <ul style="margin: 10px 0 0 20px;">
    <li><strong>Drop-off:</strong> If you're being dropped off, please have your driver drop you off on the <strong>beach side</strong> of Gulf Boulevard, not the venue side.</li>
    <li><strong>Parking:</strong> If you're driving, you can park at the reception venue address (13435 Gulf Boulevard) and walk to the beach for the ceremony.</li>
    <li>The ceremony address is at the intersection of Gulf Blvd & 134th Ave West, right on the beautiful Madeira Beach!</li>
  </ul>
</div>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Dress Code</h3>
<p><strong>Semi-Formal Beach Attire</strong> — lightweight fabrics and beach-friendly footwear recommended. It's a beach wedding in April, so it may be warm. Dress to be comfortable and celebrate with us! Semi-formal is great, but no need to be overly formal. 🌴☀️</p>
<p><strong>👡 A note on footwear:</strong> The ceremony will take place directly on the sand. We recommend block heels, wedges, sandals, or flats for comfort.</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">The Venue</h3>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; margin: 30px 0;">
  <img loading="lazy" src="/assets/images/west_events.png" alt="West Events venue exterior" style="width: 100%; border-radius: 10px;">
  <img loading="lazy" src="/assets/images/west_events2.jpg" alt="West Events venue — outdoor garden ceremony space" style="width: 100%; border-radius: 10px;">
  <img loading="lazy" src="/assets/images/west_events5.jpg" alt="West Events venue — string-light reception area" style="width: 100%; border-radius: 10px;">
  <img loading="lazy" src="/assets/images/west_events7.jpg" alt="West Events venue — interior dining space" style="width: 100%; border-radius: 10px;">
</div>

<p>The West Events is a beautiful waterfront venue in Madeira Beach, just steps from the beach! The industrial-chic space offers indoor and outdoor areas, creating the perfect backdrop for our celebration.</p>

<p><strong>Getting There:</strong> The venue is located on Gulf Boulevard in Madeira Beach, close to St. Pete - about 30 minutes from Tampa International Airport (TPA) or 20 minutes from St. Pete-Clearwater International Airport (PIE).</p>

<p><strong>Important:</strong> Parking is limited to 20 vehicles at the venue. We encourage carpooling or using rideshare services when possible!</p>

<p><strong>Uber/Rideshare Tip:</strong> If using Uber or Lyft, we recommend requesting drop-off on the <strong>beach side</strong> of the venue rather than the venue entrance. This will make it easier for you to access the ceremony location and avoid congestion at the main entrance.</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Schedule</h3>

<p><strong>More details coming soon!</strong> We'll update this with the full timeline as our plans are finalized.</p>

<ul style="margin-left: 30px;">
  <li>Ceremony</li>
  <li>Cocktail hour</li>
  <li>Reception & dinner</li>
  <li>Dancing & celebration</li>
</ul>

<div style="text-align: right; margin-top: 30px;">
  <a href="#top" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section" id="wedding-party">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Wedding Party</h2>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Bride's Side</h3>

<div style="display: grid; gap: 25px; margin: 30px 0;">

  <!-- Devlyn Parsons -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/me_dev.jpg" alt="Devlyn Parsons" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Devlyn Parsons <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Co-Maid of Honor</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Dev has been one of my best friends for about 10 years! We met at my first job out of college in Scottsdale, AZ, and our friendship stayed strong even after I moved back to California. In 2023, she moved to Clearwater and I followed to Saint Petersburg shortly after—now we hang out almost every week. She's like a big sister to me (and introduces me as her little sister!), and I'm so grateful for her love, loyalty, and support. I'm truly lucky to have her as one of my co-maids of honor!</p>
    </div>
  </div>

  <!-- Holly Smith -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/me_holly.jpg" alt="Holly Smith" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Holly Smith <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Co-Maid of Honor</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Holly and I have been friends since sophomore year of high school—over 20 years! (I used to steal her gum and cheat off her history homework ;)) She's one of the most loyal, kind, and fun people I've ever known, always there for the people she loves and incredibly strong through it all. She's a sister from another mister, and I'm so honored to have her as my other co-maid of honor!</p>
    </div>
  </div>

  <!-- Katie Ocasion -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/me_katie.jpg" alt="Katie Ocasion" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Katie Ocasion <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Katie and I have known each other since I was about 16, but our friendship really took off when I moved back to California in 2020. We bonded over a shared love of learning, growing, and reading—she totally set my book-obsessed side free! ;) She's one of the sweetest, most loyal, and fun people I know, and I'm thrilled to have her in my bridal party!</p>
    </div>
  </div>

  <!-- Emma Breneisen -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/me_emma.jpg" alt="Emma Breneisen" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Emma Breneisen <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Emma is dating Jared's brother Kegan, and I'm so lucky she's going to be my future sister-in-law! She's sweet, adventurous, crafty, smart, and so much fun—and she welcomed me with open arms from day one. She also introduced me to The Junior League of Saint Petersburg, where we both joined in 2025, so we get to spend time together most weeks. I'm thrilled to have her standing by my side on our big day!</p>
    </div>
  </div>

  <!-- Stephanie Berlinghoff -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/me_steph.jpg" alt="Stephanie Berlinghoff" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Stephanie Berlinghoff <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Stephanie and I met in kindergarten—over 30 years ago! Her family became my second family growing up, with countless camping trips and even a cruise we boarded on her 19th birthday. She's always fun to be around, and no matter how much time passes between visits, it feels like no time at all when we reconnect. I was honored to be a bridesmaid in her wedding, and I'm so grateful to have her in mine!</p>
    </div>
  </div>

  <!-- Judy Du -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/me_judy.jpg" alt="Judy Du" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Judy Du <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Judy and I met during the last year of my graduate program at UC Davis, where we both worked with our advisor, Dr. Arsuaga. We reconnected after I moved back to California in 2021 and have been close ever since—with adventures together in SoCal, Princeton, New York, and even here in Florida! She's silly, kind, and adventurous, and also an amazing listener who's always there when you need her. I'm so happy to have her in our wedding party!</p>
    </div>
  </div>

</div>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Groom's Side</h3>

<div style="display: grid; gap: 25px; margin: 30px 0;">

  <!-- Trevor Shemka -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/jared_trevor.jpg" alt="Trevor Shemka" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Trevor Shemka <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Best Man</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Trevor and Jared were college roommates and have shared many adventures since. He recently came to visit us in Florida, and it was wonderful getting to know him better—plus, he and Jared still talk on the phone all the time! Trevor is fun, kind, and supportive, and we're so glad to have him standing beside Jared on our special day!</p>
    </div>
  </div>

  <!-- Andrew Clark -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/jared_andrew.jpg" alt="Andrew Clark" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Andrew Clark <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Andrew is Jared's longest friend—they've known each other since grade school! He's a supportive, kind, and loyal friend, a great dad to two, and knows Jared better than Jared knows himself. Such a joy to have him in our wedding party!</p>
    </div>
  </div>

  <!-- Kegan Copenhagen -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/jared_kegan.jpg" alt="Kegan Copenhagen" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Kegan Copenhagen <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Kegan is Jared's younger brother—sweet, fun, and absolutely obsessed with fishing and golfing! He knows what he wants and is always there for Jared when it counts. I'm so grateful to call him my future brother-in-law and thrilled to have him standing beside Jared on our big day!</p>
    </div>
  </div>

  <!-- Chase Howard -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/jared_chase.jpg" alt="Chase Howard" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Chase Howard <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Chase is another of Jared's younger brothers—sweet, fun to hang out with, and a good man always chasing his next challenge or hustle (and crushing it). So glad to call him my future brother-in-law and have him standing beside Jared on our big day!</p>
    </div>
  </div>

  <!-- Christian Arellano -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img loading="lazy" src="/assets/images/jared_christian.JPG" alt="Christian Arellano" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Christian Arellano <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Last but not least is Christian, my nephew (my sister Ginger's son)! I've known him his whole life—which, funny enough, is most of mine too—and we grew up together like brother and sister. He's a kind spirit with a wonderful aura and an absolute delight to be around. So happy he'll be part of our special day!</p>
    </div>
  </div>

</div>

<div style="text-align: right; margin-top: 30px;">
  <a href="#top" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section" id="travel-info">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Travel & Activities</h2>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Where to Stay</h3>

<p>We know many of you are traveling from out of state! Here are our recommended hotels near the venue, listed by distance:</p>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">📍 Things to Know Before Booking</h4>

<p>The St. Pete area has several distinct neighborhoods, each with a different vibe. Here's a quick guide to help you pick the right spot:</p>

<ul style="margin-left: 30px;">
  <li><strong>Madeira Beach / Treasure Island</strong> — <em>Closest to the venue.</em> We highly recommend looking up where <strong>The West Events</strong> (13435 Gulf Boulevard, Madeira Beach) is on a map and doing your best to stay as close as possible. The closer you are, the easier it'll be to get to and from the festivities!</li>
  <li><strong>St. Pete Beach</strong> — More of a resort-style area with larger beachfront hotels. A short drive from the venue.</li>
  <li><strong>Downtown St. Pete</strong> — Great for nightlife and restaurants, but farther from the venue (about 25-30 minutes away).</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 25px;">🏡 Our Top Recommendation: Vacation Rentals (Airbnb & VRBO)</h4>

<p><strong>If you're traveling with a group, family, or friends, we highly recommend booking a vacation rental!</strong> There are tons of beachfront and near-beach homes and condos on Airbnb and VRBO right near the venue, and splitting a house together is hands-down the most fun (and often most affordable) way to enjoy the weekend in our area. Madeira Beach, Treasure Island, and the surrounding neighborhoods have plenty of great options.</p>

<p><strong>💡 Tip:</strong> Try to book as close to <strong>The West Events</strong> (13435 Gulf Boulevard, Madeira Beach) as possible so you're near the ceremony and reception.</p>

<ul style="margin-left: 30px;">
  <li><a href="https://www.airbnb.com/s/Madeira-Beach--FL/homes" target="_blank" rel="noopener">Search Airbnb in Madeira Beach</a></li>
  <li><a href="https://www.vrbo.com/vacation-rentals/usa/florida/central-west/madeira-beach" target="_blank" rel="noopener">Search VRBO in Madeira Beach</a></li>
  <li><a href="https://www.vrbo.com/search?latLong=27.78564%2C-82.78372&mapBounds=27.78238%2C-82.78767&mapBounds=27.7889%2C-82.77977&startDate=2027-04-14&endDate=2027-04-18&adults=8&children=1_17%2C1_17&sort=RECOMMENDED" target="_blank" rel="noopener">Search VRBO rentals near the venue (pre-filtered for our wedding dates)</a></li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 25px;">⭐ Venue Partner Hotels (Discounts Available!)</h4>

<p>Prefer a hotel? The West Events partners with these nearby hotels, offering exclusive discounts and amenities for our guests. Mention <strong>The West Events</strong> when booking!</p>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin: 20px 0;">

  <div style="background: #f8f4ec; padding: 20px; border-left: 4px solid #d4a574; border-radius: 5px;">
    <h4 style="color: #2c5f6f; margin: 0 0 10px 0; font-size: 1.15em;">Cambria Hotel Madeira Beach</h4>
    <p style="margin: 5px 0;"><strong>Contact:</strong> Sohnne Sanz, Director of Sales</p>
    <p style="margin: 5px 0;"><strong>Phone:</strong> (727) 350-7332</p>
    <p style="margin: 5px 0;"><strong>Email:</strong> sohnne@bowdenhospitality.com</p>
    <p style="margin: 5px 0;"><a href="https://www.cambriamadeirabeach.com" target="_blank" rel="noopener">cambriamadeirabeach.com</a></p>
  </div>

  <div style="background: #f8f4ec; padding: 20px; border-left: 4px solid #d4a574; border-radius: 5px;">
    <h4 style="color: #2c5f6f; margin: 0 0 10px 0; font-size: 1.15em;">Barefoot Beach Club</h4>
    <p style="margin: 5px 0;"><strong>Contact:</strong> Amanda, Event Sales</p>
    <p style="margin: 5px 0;"><strong>Phone:</strong> (727) 393-6133</p>
    <p style="margin: 5px 0;"><strong>Email:</strong> amanda@barefootbeachclub.com</p>
    <p style="margin: 5px 0;"><strong>Discount Code:</strong> <span style="background: #d4a574; color: white; padding: 2px 8px; border-radius: 3px; font-weight: bold;">WEST15</span> (15% off online)</p>
    <p style="margin: 5px 0;"><a href="https://barefootbeachclub.com/" target="_blank" rel="noopener">barefootbeachclub.com</a></p>
  </div>

  <div style="background: #f8f4ec; padding: 20px; border-left: 4px solid #d4a574; border-radius: 5px;">
    <h4 style="color: #2c5f6f; margin: 0 0 10px 0; font-size: 1.15em;">DoubleTree Beach Resort – Redington Beach</h4>
    <p style="margin: 5px 0;"><strong>Contact:</strong> Marie Molina, Catering & Event Sales</p>
    <p style="margin: 5px 0;"><strong>Phone:</strong> (727) 369-7139</p>
    <p style="margin: 5px 0;"><strong>Email:</strong> Marie.Molina@hilton.com</p>
    <p style="margin: 5px 0;"><strong>Discount:</strong> Ask Marie about group discounts</p>
    <p style="margin: 5px 0;"><a href="https://www.hilton.com/en/book/reservation/deeplink/?ctyhocn=NORNHDT&corporateCode=0003252998" target="_blank" rel="noopener">Book with corporate rate</a></p>
  </div>

  <div style="background: #f8f4ec; padding: 20px; border-left: 4px solid #d4a574; border-radius: 5px;">
    <h4 style="color: #2c5f6f; margin: 0 0 10px 0; font-size: 1.15em;">Courtyard Marriott St. Petersburg Clearwater/Madeira Beach</h4>
    <p style="margin: 5px 0;"><a href="https://www.marriott.com/event-reservations/reservation-link.mi?id=16698130%2022393&key=CORP&app=resvlink" target="_blank" rel="noopener">Book with TWE corporate rate</a></p>
  </div>

</div>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 25px;">Other Nearby Options</h4>

<p><strong>Madeira Beach (walking distance to 1 mile):</strong></p>
<ul style="margin-left: 30px;">
  <li>Inn on the Beach - Boutique beachfront hotel</li>
  <li>Madeira Bay Resort - Condo-style suites with kitchens</li>
  <li>Sea Breeze Suites - Budget-friendly option</li>
</ul>

<p><strong>Treasure Island (2-3 miles):</strong></p>
<ul style="margin-left: 30px;">
  <li>Thunderbird Beach Resort - Classic beach hotel</li>
  <li>Bilmar Beach Resort - Family-friendly beachfront</li>
  <li>Alden Beach Resort - Suites with kitchens</li>
  <li>Treasure Island Beach Resort - Beachfront property</li>
</ul>

<p><strong>North Redington Beach (2-3 miles):</strong></p>
<ul style="margin-left: 30px;">
  <li>Doubletree Beach Resort by Hilton - Mid-range beachfront</li>
</ul>

<p><strong>St. Pete Beach (5-7 miles):</strong></p>
<ul style="margin-left: 30px;">
  <li>Grand Plaza Beachfront Resort - Mid-range beachfront</li>
  <li>Sirata Beach Resort - Family-friendly with multiple pools</li>
  <li>TradeWinds Island Grand - Large resort with activities</li>
  <li>The Don CeSar - Iconic pink palace, luxury option</li>
</ul>

<p style="font-style: italic;">We'll be setting up hotel blocks - check back for booking codes!</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Getting Around St. Pete</h3>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">Airports</h4>
<p>There are two convenient airport options for flying into the area:</p>
<ul style="margin-left: 30px;">
  <li><strong>Tampa International Airport (TPA):</strong> The largest airport in the region, with the most flight options. About 30 minutes from Madeira Beach.</li>
  <li><strong>St. Pete-Clearwater International Airport (PIE):</strong> A smaller, closer airport - about 20 minutes from Madeira Beach. <strong>Especially convenient for guests flying from Michigan</strong>, as Allegiant offers direct flights from Flint (FNT) to St. Pete (PIE)!</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">Transportation Options</h4>

<ul style="margin-left: 30px;">
  <li><strong>Uber/Lyft:</strong> Readily available throughout St. Petersburg</li>
  <li><strong>Rental Cars:</strong> Available at both Tampa International Airport (TPA) and St. Pete-Clearwater International Airport (PIE)</li>
  <li><strong>Looper Trolley:</strong> Free downtown trolley service</li>
  <li><strong>Scooters/Bikes:</strong> Bird and Lime scooters available throughout the city</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">Parking at Venue</h4>
<p><strong>Important:</strong> The venue can accommodate a maximum of 20 cars. We strongly encourage:</p>
<ul style="margin-left: 30px;">
  <li>Carpooling with other guests</li>
  <li>Using rideshare services (Uber/Lyft)</li>
  <li>Staying at a nearby hotel and taking a short ride</li>
</ul>

<p><strong>We highly recommend staying nearby and using Uber/Lyft to the venue.</strong> Parking is extremely limited and rideshare will be the easiest option for most guests.</p>

<p>You're also welcome to rent a car to get around the area more easily during your stay. If you do, please <strong>carpool with other guests</strong> heading to the venue and <strong>check in with us ahead of time</strong> so we know how many cars to expect at the venue.</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Things to do in St. Pete</h3>

<p>Whether you're here for the weekend or making a vacation of it, here are some of our favorite spots:</p>

<p><strong>Beaches:</strong></p>
<ul style="margin-left: 30px;">
  <li>St. Pete Beach</li>
  <li>Madeira Beach</li>
  <li>Pass-a-Grille Beach</li>
</ul>

<p><strong>Attractions:</strong></p>
<ul style="margin-left: 30px;">
  <li>The Pier</li>
  <li>Dali Museum</li>
  <li>Vinoy Park</li>
  <li>Sunken Gardens</li>
  <li>Downtown St. Pete</li>
  <li>Museum of Fine Arts</li>
</ul>

<p><strong>Activities:</strong></p>
<ul style="margin-left: 30px;">
  <li>Paddleboarding</li>
  <li>Beach volleyball</li>
  <li>Shopping on Beach Drive</li>
  <li>Art galleries in the EDGE District</li>
</ul>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 30px;">🌴 BEST "Wedding Weekend" Recommendations</h3>

<p>If you're making a weekend (or week!) of it, here are our favorite local spots — very Florida, very fun.</p>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">🌅 Best Sunset Spots</h4>
<ul style="margin-left: 30px;">
  <li><strong>Pass-a-Grille Beach</strong> — Our top recommendation. Charming, walkable, quieter, and beautiful sunsets.</li>
  <li><strong>Upham Beach</strong> — Great for a classic beach afternoon.</li>
  <li><strong>Sunset Beach</strong> — Fun, relaxed, local vibe.</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">🍹 Fun Casual Beach Bars & Hangouts</h4>
<ul style="margin-left: 30px;">
  <li><strong>Caddy's Treasure Island</strong> — Very beachy Florida atmosphere.</li>
  <li><strong>Jimmy B's Beach Bar</strong> — Live music and a great beach vibe.</li>
  <li><strong>Saltwater Hippie</strong> — Cute coastal aesthetic and good drinks.</li>
  <li><strong>The Toasted Monkey</strong> — Fun brunch and casual stop.</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">☕ Coffee & Morning Spots</h4>
<ul style="margin-left: 30px;">
  <li><strong>The Grove Surf + Coffee</strong> — Adorable coastal café.</li>
  <li><strong>Bandit Coffee Co.</strong> — Popular local favorite.</li>
  <li><strong>Pete's Bagels</strong> — Amazing breakfast option.</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">🍽️ BEST Dinner Recommendations</h4>
<ul style="margin-left: 30px;">
  <li><strong>Juno & The Peacock</strong> — Great upscale option.</li>
  <li><strong>Salt Rock Grill</strong> — Classic waterfront Florida dinner.</li>
  <li><strong>Doc Ford's Rum Bar & Grille</strong> — Fun for groups and visitors.</li>
  <li><strong>Allelo</strong> — More modern, date-night vibe.</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">🎨 Best Things To Do</h4>
<ul style="margin-left: 30px;">
  <li><strong>St. Pete Pier</strong> — A MUST for visitors.</li>
  <li><strong>The Dalí Museum</strong> — One of the best museums in Florida.</li>
  <li><strong>Sunken Gardens</strong> — Beautiful for slower mornings.</li>
  <li><strong>John's Pass Village & Boardwalk</strong> — Touristy but very fun for out-of-towners.</li>
</ul>

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 25px;">💛 Our Favorites</h4>
<p>If you want to experience a little piece of <em>us</em> while you're in town, here are some of our most-loved spots:</p>
<ul style="margin-left: 30px;">
  <li><strong>Bad Mother</strong> — The coffee shop where Jared and I met on our first date ☕</li>
  <li><strong>Doc Ford's</strong> — Where we had lunch on our first date 🥂</li>
  <li><strong>The Lure</strong> — Our favorite date-night restaurant 🍽️</li>
  <li><strong>The Library</strong> — Our favorite brunch spot 🥞</li>
  <li><strong>Caddy's on Madeira Beach</strong> — Our favorite beachfront restaurant 🏖️</li>
  <li><strong>The Book Lounge</strong> — A bookstore Rachael loves, with fun games, drinks, and snacks 📚</li>
  <li><strong>Book & Bottle</strong> — Another favorite bookstore of Rachael's with great drinks and snacks 🍷</li>
  <li><strong>Madeira Beach</strong> — Our favorite spot to catch the sunset 🌅</li>
</ul>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Where to Eat</h3>

<p>Here are some of our favorite restaurants in the area:</p>

<p><strong>Casual:</strong></p>
<ul style="margin-left: 30px;">
  <li>The Lure</li>
  <li>Doc Ford's - on the Pier</li>
  <li>Boardwalk Burgers & Fries</li>
  <li>Pizza Bella</li>
</ul>

<p><strong>Nice Dinner:</strong></p>
<ul style="margin-left: 30px;">
  <li>Juno & The Peacock</li>
  <li>Sea-Gals Restaurant & Lounge</li>
  <li>Sloppy Joe's on the Beach</li>
  <li>Salt Rock Grill</li>
  <li>Sculley's</li>
</ul>

<p><strong>Brunch:</strong></p>
<ul style="margin-left: 30px;">
  <li>Juno & The Peacock</li>
  <li>The Breakfast Station</li>
  <li>The Gallery</li>
  <li>Cafe 118</li>
</ul>

<div style="text-align: right; margin-top: 30px;">
  <a href="#top" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section" id="rsvp">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">RSVP</h2>

<p style="text-align:center; font-size:1.15em; margin: 10px 0 20px;"><strong>💌 Please RSVP by <span style="color:#d4a574;">January 25, 2027</span></strong></p>

<p style="font-style: italic; color: #555;">Formal invitations with mailing details will go out closer to the date — but if you already know you're coming (or can't make it), please let us know below! It helps us with planning.</p>

<!--
  RSVP — embedded Google Form. Responses land in:
    https://docs.google.com/forms/d/e/1FAIpQLScKSylvxHERAHJtR7vdQC_3q6SAirCB8gENc9fjj485c4sWTg/viewform
  To swap to a different form later, replace the iframe src below.
-->

<div style="background: linear-gradient(135deg, #fdf6ec 0%, #ffffff 100%); padding: 24px; border-radius: 14px; box-shadow: 0 6px 20px rgba(0,0,0,0.08); max-width: 760px; margin: 20px auto;">
  <iframe
    src="https://docs.google.com/forms/d/e/1FAIpQLScKSylvxHERAHJtR7vdQC_3q6SAirCB8gENc9fjj485c4sWTg/viewform?embedded=true"
    width="100%"
    height="1400"
    frameborder="0"
    marginheight="0"
    marginwidth="0"
    title="Wedding RSVP form"
    style="border: none; display: block; background: transparent; border-radius: 8px;">
    Loading RSVP form…
  </iframe>
</div>

<p style="text-align:center; color:#555; margin-top:18px;">Trouble with the form? Email us at <a href="mailto:rachaelapsmith@gmail.com" style="color:#2c5f6f; font-weight:bold;">rachaelapsmith@gmail.com</a></p>

<div style="text-align: right; margin-top: 30px;">
  <a href="#top" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section" id="faqs">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">FAQs</h2>

<p><strong>When should I arrive?</strong><br>
We recommend arriving the day before the wedding (April 14th) to give yourself time to settle in and explore St. Petersburg!</p>

<p><strong>What's the weather like in April?</strong><br>
April in St. Pete is beautiful! Average temperatures are in the mid-70s to low-80s°F. Perfect beach weather!</p>

<p><strong>Can I bring a plus-one?</strong><br>
Your invitation will specify if you have a plus-one. Due to venue capacity, we're unable to accommodate additional guests beyond those listed on your invitation.</p>

<p><strong>Is there parking at the venue?</strong><br>
Parking is very limited (maximum 20 vehicles). We strongly encourage using Uber/Lyft or carpooling with other guests.</p>

<p><strong>Are kids welcome?</strong><br>
Due to venue capacity, we can only accommodate children who are nieces/nephews of the bride and groom. We appreciate your understanding!</p>

<p><strong>What if I have dietary restrictions?</strong><br>
Please let us know on your RSVP card, and we'll make sure you're taken care of!</p>

<p><strong>Will there be an open bar?</strong><br>
Beer and wine will be hosted during the first two hours of the reception, followed by a cash bar. Signature cocktails and mocktails will also be available!</p>

<p><strong>What time should I leave?</strong><br>
The reception will go until approximately 10:00 PM. Party as long as you'd like!</p>

<div style="text-align: right; margin-top: 30px;">
  <a href="#top" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Questions?</h2>

<p>Have questions we didn't answer? Feel free to reach out:</p>

<p>📧 Email: rachaelapsmith@gmail.com<br>
💌 Or message us directly!</p>

<p style="text-align: center; font-size: 1.3em; margin-top: 30px; font-style: italic; color: #2c5f6f;">We can't wait to celebrate with you! 💕</p>

</div>

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
      var elD = document.getElementById('wcd-days');
      var elH = document.getElementById('wcd-hours');
      var elM = document.getElementById('wcd-mins');
      var elS = document.getElementById('wcd-secs');
      if (elD) elD.textContent = d;
      if (elH) elH.textContent = h;
      if (elM) elM.textContent = m;
      if (elS) elS.textContent = s;
    }
    tick();
    setInterval(tick, 1000);
  })();
</script>

