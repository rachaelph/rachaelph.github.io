---
layout: page
permalink: /wedding/
---

<style>
  /* Elegant wedding page styling */
  
  /* Sandy background for entire page */
  body {
    background-color: #F5DEB3 !important;
  }
  
  /* Override theme width constraints */
  .page__content,
  .page-content,
  article,
  main {
    max-width: 100% !important;
    margin-left: auto !important;
    margin-right: auto !important;
    background-color: #F5DEB3;
  }
  
  .wedding-page {
    font-family: 'Georgia', 'Garamond', serif;
    background-color: #F5DEB3;
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

<div class="wedding-page" style="padding: 20px 0;">

<div style="display: flex; gap: 40px; align-items: center; margin: 40px auto; max-width: 1200px; padding: 0 20px; flex-wrap: wrap;">
  
  <div style="flex: 1; min-width: 280px;">
    <div class="our-wedding-title" style="text-align: left; margin: 0 0 20px 0;">
      <h1 style="font-family: 'Great Vibes', 'Playfair Display', 'Georgia', cursive; font-size: 3em; color: #0d8a9a; margin: 0; font-weight: 400; letter-spacing: 2px;">Our Wedding</h1>
    </div>
    
    <div class="wedding-title" style="text-align: left;">
      <h1 style="color: #00695C; font-size: 1.8em; margin-bottom: 10px; font-weight: normal; letter-spacing: 2px;"> Rachael & Jared </h1>
      <h2 style="color: #2c5f6f; font-size: 1.5em; font-weight: 300; margin: 5px 0;"> April 15, 2027 </h2>
      <p style="color: #666; font-size: 1.2em; font-style: italic;"> Madeira Beach, Florida </p>
    </div>
  </div>
  
  <div style="flex: 0 0 350px; min-width: 280px; max-width: 100%;">
    <img src="/assets/images/wedding_logo.png" alt="Rachael & Jared Wedding Logo" style="max-width: 100%; width: 100%; height: auto;">
  </div>
  
</div>

<!-- Engagement Photo -->
<div style="text-align: center; margin: 40px auto;">
  <img src="/assets/images/engagementphotos8.jpeg" alt="Rachael and Jared" style="max-width: 600px; width: 100%; border-radius: 15px; box-shadow: 0 6px 20px rgba(0,0,0,0.2);">
</div>

<!-- Quick Links Navigation -->
<div style="background: rgba(255, 255, 255, 0.95); padding: 20px; margin: 30px auto; text-align: center; box-shadow: 0 4px 15px rgba(0,0,0,0.1); max-width: 1000px; border-radius: 10px;">
  <p style="color: #2c5f6f; font-weight: bold; margin-bottom: 15px; font-size: 1.1em;">Quick Links</p>
  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; padding: 0 10px;">
    <a href="#event-details" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Venue & Schedule</a>
    <a href="#wedding-party" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Wedding Party</a>
    <a href="#travel-info" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Travel & Activities</a>
    <a href="#honeymoon-fund" style="background: #d4a574; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">Honeymoon Fund 🌴</a>
    <a href="#rsvp" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">RSVP</a>
    <a href="#faqs" style="background: #2c5f6f; color: white; padding: 6px 12px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.85em; transition: background 0.3s;">FAQs</a>
  </div>
</div>

<div class="wedding-section" id="event-details">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Venue & Schedule</h2>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Event Details</h3>

<p><strong>📅 Date:</strong> Thursday, April 15, 2027<br>
<strong>🕐 Ceremony:</strong> 4:00 or 5:00 PM (final time TBD)<br>
<strong>📍 Venue:</strong> <a href="https://www.thewesteventspace.com/" target="_blank">The West Events</a><br>
<strong>🏠 Address:</strong> 13435 Gulf Boulevard, Madeira Beach, FL 33708<br>
<strong>📞 Phone:</strong> (727) 363-4255</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Dress Code</h3>
<p><strong>Semi-Formal Beach Attire</strong> - Think beachy colors and lightweight fabrics! It's a beach wedding in April, so it may be warm. Dress to be comfortable and celebrate with us! Semi-formal is great, but no need to be overly formal. 🌴☀️</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">The Venue</h3>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; margin: 30px 0;">
  <img src="/assets/images/west_events.png" alt="Venue" style="width: 100%; border-radius: 10px;">
  <img src="/assets/images/west_events3.jpg" alt="Venue 3" style="width: 100%; border-radius: 10px;">
  <img src="/assets/images/west_events5.jpg" alt="Venue 5" style="width: 100%; border-radius: 10px;">
  <img src="/assets/images/west_events7.jpg" alt="Venue 7" style="width: 100%; border-radius: 10px;">
</div>

<p>The West Events is a beautiful waterfront venue in Madeira Beach, just steps from the beach! The industrial-chic space offers indoor and outdoor areas, creating the perfect backdrop for our celebration.</p>

<p><strong>Getting There:</strong> The venue is located on Gulf Boulevard in Madeira Beach, close to St. Pete and about 30 minutes from Tampa International Airport (TPA).</p>

<p><strong>Important:</strong> Parking is limited to 20 vehicles at the venue. We encourage carpooling or using rideshare services when possible!</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Schedule</h3>

<p><strong>More details coming soon!</strong> We'll update this with the full timeline as our plans are finalized.</p>

<ul style="margin-left: 30px;">
  <li>Ceremony</li>
  <li>Cocktail hour</li>
  <li>Reception & dinner</li>
  <li>Dancing & celebration</li>
</ul>

<div style="text-align: right; margin-top: 30px;">
  <a href="#" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section" id="wedding-party">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Wedding Party</h2>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Bride's Side</h3>

<div style="display: grid; gap: 25px; margin: 30px 0;">

  <!-- Devlyn Parsons -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/me_dev.jpg" alt="Devlyn Parsons" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Devlyn Parsons <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Co-Maid of Honor</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Dev has been one of my best friends for roughly 10 years! We met at my first job out of college in Scottsdale, AZ, and quickly became close friends. I moved back to California to help my dad for three years at the end of 2020, but our friendship stayed strong. At the beginning of 2023, Dev moved to Clearwater, Florida, and several months later, I moved to Saint Petersburg! We were reunited and now hang out all the time—about once a week, if not more. She is like a big sister to me, and when she introduces me, she calls me her little sister! I am so grateful for her love, support, kindness, and loyalty. She is an amazing sister and friend, and I am truly lucky to have her as one of my co-maids of honor!</p>
    </div>
  </div>

  <!-- Holly Smith -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/me_holly.jpg" alt="Holly Smith" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Holly Smith <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Co-Maid of Honor</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Holly and I have been friends since sophomore year of high school, over 20 years! I used to steal her gum and cheat off her history homework ;) She is one of the most loyal, understanding, kind, and fun people I have ever had the pleasure of knowing! She is always there for the people she loves and will do anything for those she cares about. She's incredibly strong and resilient, and she's another sister from another mister to me! I am so honored and grateful to have her as my other co-maid of honor!</p>
    </div>
  </div>

  <!-- Katie Ocasion -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/me_katie.jpg" alt="Katie Ocasion" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Katie Ocasion <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Katie and I have known each other since I was about 16 years old. We weren't very close at first, but when I moved back to California at the end of 2020, everything changed! We started bonding over our shared love of learning, growing, and reading. If you know anything about me, you know I'm obsessed with books and reading... Katie totally set that part of me free! ;) She's not only a wonderful book buddy, but also one of the sweetest, most fun, loyal, and wonderful people I know. I'm so grateful our friendship has grown the way it has and thrilled to have her as part of my bridal party for this joyous occasion!</p>
    </div>
  </div>

  <!-- Emma Breneisen -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/me_emma.jpg" alt="Emma Breneisen" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Emma Breneisen <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Emma is dating Jared's brother Kegan, and I'm so lucky she's going to be my future sister-in-law! She is such a sweet, adventurous, crafty, social, smart, stylish, and fun woman. From the moment Jared and I started dating, she welcomed me with open arms. She also introduced me to The Junior League of Saint Petersburg, a women's non-profit organization we both joined in 2025! Now we're both actively involved with the chapter and get to spend time together most weeks—whether at Junior League events, family gatherings, or just hanging out. I'm thrilled to have her standing by my side on our big day!</p>
    </div>
  </div>

  <!-- Stephanie Berlinghoff -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/me_steph.jpg" alt="Stephanie Berlinghoff" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Stephanie Berlinghoff <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Stephanie and I met in kindergarten—we've known each other for over 30 years! During our childhood and teenage years, her family became my second family, and I spent countless hours on trips with them. We went camping multiple times and even went on a cruise that we boarded on Stephanie's 19th birthday! She's always been so fun to be around and knows how to not take life too seriously. Even when months have passed without talking, when we reconnect, it's like no time has passed at all! I was honored to be a bridesmaid in her wedding, and I'm so grateful she's part of my bridal party as well!</p>
    </div>
  </div>

  <!-- Judy Du -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/me_judy.jpg" alt="Judy Du" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Judy Du <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Bridesmaid</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Judy and I met during the last year of my graduate program at UC Davis, where we both worked with our advisor, Dr. Arsuaga. We were friends, but not close friends... yet! Years later, we reconnected when I moved back to California in 2021. She was living in SoCal, so I drove down to hang out with her, and we've been great friends ever since! I've visited her in SoCal, Princeton, and New Jersey/New York, where we went on SO many adventures together. She's even come to Florida to visit Jared and me! I absolutely love hanging out and traveling with her. She's super silly, fun, kind, and adventurous—she knows how to not take life too seriously, but she's also an amazing listener who's always there when you need her. I'm so happy to have her in our wedding party!</p>
    </div>
  </div>

</div>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Groom's Side</h3>

<div style="display: grid; gap: 25px; margin: 30px 0;">

  <!-- Trevor Shemka -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/jared_trevor.jpg" alt="Trevor Shemka" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Trevor Shemka <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Best Man</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Trevor and Jared were roommates in college and have shared many fun adventures together over the years! He even came to visit us in Florida recently, and it was wonderful getting to know him better. They talk frequently on the phone, which is awesome to see! Trevor is a fun, kind, and supportive guy, and we're so glad to have him standing beside Jared on this special day!</p>
    </div>
  </div>

  <!-- Andrew Clark -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/jared_andrew.jpg" alt="Andrew Clark" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Andrew Clark <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Andrew is Jared's longest friend—they've known each other since grade school! From what I hear, Andrew is a supportive, kind, and loyal friend. He is also a great dad to two children! He's always there for Jared and knows him better than Jared knows himself! It's such a joy to have him in our wedding party!</p>
    </div>
  </div>

  <!-- Kegan Copenhagen -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/jared_kegan.jpg" alt="Kegan Copenhagen" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Kegan Copenhagen <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Kegan is Jared's younger brother! He's sweet, fun, and absolutely obsessed with fishing and golfing. He's definitely stubborn and knows what he wants, but he's always there for Jared when he needs him. I'm so grateful to call him my future brother-in-law and thrilled he'll be standing beside Jared on this special day!</p>
    </div>
  </div>

  <!-- Chase Howard -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/jared_chase.jpg" alt="Chase Howard" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Chase Howard <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Chase is another one of Jared's younger brothers! He's sweet, fun to hang out with, and a good man. He's always looking for his next challenge or money-making hustle, which he is very good at! I'm so glad to call him my future brother-in-law and thrilled to have him standing beside Jared on our big day!</p>
    </div>
  </div>

  <!-- Christian Arellano -->
  <div style="display: flex; gap: 20px; align-items: flex-start; flex-wrap: wrap;">
    <img src="/assets/images/jared_christian.JPG" alt="Christian Arellano" style="width: 250px; max-width: 100%; height: 250px; object-fit: cover; border-radius: 10px; flex-shrink: 0; image-rendering: -webkit-optimize-contrast; image-rendering: crisp-edges;">
    <div>
      <h4 style="color: #2c5f6f; margin: 0 0 5px 0; font-size: 1.3em;">Christian Arellano <span style="color: #d4a574; font-size: 0.85em; font-style: italic;">- Groomsman</span></h4>
      <p style="color: #00695C; line-height: 1.6;">Last but not least is Christian, my nephew (my sister Ginger's son)! I've known him his whole life—which, funny enough, is most of my life too. We grew up together like brother and sister! He's such a kind spirit with a wonderful aura and is an absolute delight to hang out with. I'm so happy he's going to be part of our special day!</p>
    </div>
  </div>

</div>

<div style="text-align: right; margin-top: 30px;">
  <a href="#" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section" id="travel-info">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Travel & Activities</h2>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">Where to Stay</h3>

<p>We know many of you are traveling from out of state! Here are our recommended hotels near the venue, listed by distance:</p>

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

<h4 style="color: #2c5f6f; font-size: 1.2em; margin-top: 20px;">Transportation Options</h4>

<ul style="margin-left: 30px;">
  <li><strong>Uber/Lyft:</strong> Readily available throughout St. Petersburg</li>
  <li><strong>Rental Cars:</strong> Available at Tampa International Airport (TPA) - about 30 minutes from St. Pete</li>
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
  <a href="#" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<!-- Honeymoon Fund Section -->
<div class="wedding-section" id="honeymoon-fund">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">Honeymoon Fund 🌴</h2>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin: 30px 0;">
  <img src="/assets/images/costa_rica.jpg" alt="Costa Rica" style="width: 100%; height: 250px; object-fit: cover; border-radius: 10px;">
  <img src="/assets/images/costa_rica2.jpg" alt="Costa Rica" style="width: 100%; height: 250px; object-fit: cover; border-radius: 10px;">
  <img src="/assets/images/costa_rica3.jpg" alt="Costa Rica" style="width: 100%; height: 250px; object-fit: cover; border-radius: 10px;">
  <img src="/assets/images/costa_rica5.jpg" alt="Costa Rica" style="width: 100%; height: 250px; object-fit: cover; border-radius: 10px;">
  <img src="/assets/images/costa_rica6.jpg" alt="Costa Rica" style="width: 100%; height: 250px; object-fit: cover; border-radius: 10px;">
  <img src="/assets/images/costa_rica7.jpg" alt="Costa Rica" style="width: 100%; height: 250px; object-fit: cover; border-radius: 10px;">
</div>

<p>The greatest gift to us is your presence on our special day! However, if you would like to contribute to our honeymoon, we would be so grateful. We're planning an amazing 10-day adventure to <strong>Costa Rica</strong>!</p>

<p>Instead of a traditional registry, we're asking for help funding our dream honeymoon. Your contribution will help us create unforgettable memories as we start our married life together.</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;">How to Contribute</h3>

<p>Choose the payment method that works best for you:</p>

<div style="background: #f5f5f5; padding: 30px; border-radius: 10px; margin: 30px 0;">
  
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px;">
    
    <div style="text-align: center; padding: 15px;">
      <p style="font-size: 1.1em; margin-bottom: 10px;"><strong> Venmo </strong></p>
      <img src="/assets/images/venmo.png" alt="Venmo QR Code" style="width: 150px; height: 150px; margin: 10px auto; display: block;">
    </div>
    
    <div style="text-align: center; padding: 15px;">
      <p style="font-size: 1.1em; margin-bottom: 10px;"><strong> Zelle </strong></p>
      <p style="font-size: 0.95em; color: #00695C; font-weight: bold; word-wrap: break-word;">rachael.phillips23@<br>gmail.com</p>
    </div>
    
    <div style="text-align: center; padding: 15px;">
      <p style="font-size: 1.1em; margin-bottom: 10px;"><strong> CashApp </strong></p>
      <p style="font-size: 1.1em; color: #00695C; font-weight: bold; word-wrap: break-word;">$rachaelaps</p>
    </div>
    
    <div style="text-align: center; padding: 15px;">
      <p style="font-size: 1.1em; margin-bottom: 10px;"><strong> PayPal </strong></p>
      <p style="font-size: 0.95em; color: #00695C; font-weight: bold; word-wrap: break-word;">rachael.phillips23@<br>gmail.com</p>
    </div>
    
  </div>
  
  <p style="text-align: center; color: #BF9B7A; margin-top: 20px; font-style: italic;">Please include "Honeymoon Fund 💕" in the note</p>
  
</div>

<p style="background: #00697F; padding: 15px; border-radius: 8px; color: #BF9B7A;"><strong>Prefer to give a check?</strong><br>
You can make checks payable to <strong>Rachael Phillips</strong> or <strong>Jared Smith</strong> and give them to us at the wedding or mail them to us (contact us for mailing address).</p>

<h3 style="color: #2c5f6f; font-size: 1.5em; margin-top: 25px;"> Help Us Experience Costa Rica </h3>

<p>Here's what we're planning for our 10-day adventure:</p>

<p><strong>Accommodations & Travel:</strong></p>
<ul style="margin-left: 30px;">
  <li>✈️ Round-trip flights (Tampa to San Jose)</li>
  <li>🏨 Luxury resort stay (2-3 nights)</li>
  <li>🚗 AWD car rental for exploring</li>
</ul>

<p><strong>Adventures & Excursions:</strong></p>
<ul style="margin-left: 30px;">
  <li>☕ Coffee plantation tour</li>
  <li>🌋 Volcano tour and hot springs</li>
  <li>🌿 Cloud forest exploration</li>
  <li>💦 Waterfall tours and cave springs</li>
  <li>🏖️ Beach days and water activities</li>
  <li>🌅 Romantic sunset experiences</li>
</ul>

<p><strong>Special Moments:</strong></p>
<ul style="margin-left: 30px;">
  <li>🍽️ Romantic beachside dinners</li>
  <li>💆‍♀️ Couples spa day</li>
  <li>🎉 Any amount toward our dream honeymoon!</li>
</ul>

<p style="font-style: italic;">We're finalizing the specific costs for each experience - check back soon for updated pricing!</p>

<p style="font-size: 1.2em; font-weight: bold; margin-top: 20px;"><strong>Estimated Total Honeymoon Cost:</strong> $4,500 - $6,000</p>

<div style="text-align: right; margin-top: 30px;">
  <a href="#" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
</div>

</div>

<div class="wedding-section" id="rsvp">

<h2 style="color: #2c5f6f; font-size: 2em; border-bottom: 2px solid #d4a574; padding-bottom: 10px; margin-bottom: 20px; font-family: 'Georgia', serif;">RSVP</h2>

<p><strong>RSVP details coming soon!</strong> We'll be sending official invitations with RSVP instructions. Please respond by your invitation date.</p>

<p>You can also email us at rachaelapsmith@gmail.com with questions!</p>

<div style="text-align: right; margin-top: 30px;">
  <a href="#" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
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
Due to venue capacity, we can only accommodate children who are nieces/nephews of the bride and groom or children of the bridal party. We appreciate your understanding!</p>

<p><strong>What if I have dietary restrictions?</strong><br>
Please let us know on your RSVP card, and we'll make sure you're taken care of!</p>

<p><strong>Will there be an open bar?</strong><br>
Yes! We'll have beer and wine available for the first 2 hours of the reception. After that, it will be a cash bar. We'll also have signature mocktails and cocktails available (details coming soon)!</p>

<p><strong>What time should I leave?</strong><br>
The reception will go until approximately 10:00 PM (to be confirmed). Party as long as you'd like!</p>

<div style="text-align: right; margin-top: 30px;">
  <a href="#" style="background: #d4a574; color: white; padding: 8px 16px; border-radius: 5px; text-decoration: none; font-weight: bold; font-size: 0.9em; display: inline-block;">↑ Back to Top</a>
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

