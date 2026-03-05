[index.html](https://github.com/user-attachments/files/25767884/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>KiyoKanshiEdits</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Arial', sans-serif;
      background: #0a0a0f;
      color: #fff;
      min-height: 100vh;
    }
    header {
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #1a1a2e;
    }
    header .logo {
      font-size: 1.4em;
      font-weight: bold;
      letter-spacing: 2px;
      background: linear-gradient(90deg, #7b2fff, #ff3cac);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    header nav a {
      color: #aaa;
      text-decoration: none;
      margin-left: 24px;
      font-size: 0.9em;
      transition: color 0.2s;
    }
    header nav a:hover { color: #fff; }

    .hero {
      text-align: center;
      padding: 100px 20px 60px;
    }
    .hero h1 {
      font-size: 3em;
      letter-spacing: 4px;
      background: linear-gradient(90deg, #7b2fff, #ff3cac, #ff6b35);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 20px;
    }
    .hero p {
      color: #aaa;
      font-size: 1.1em;
      max-width: 500px;
      margin: 0 auto 40px;
      line-height: 1.7;
    }
    .hero a.cta {
      display: inline-block;
      padding: 14px 36px;
      background: linear-gradient(90deg, #7b2fff, #ff3cac);
      color: #fff;
      text-decoration: none;
      border-radius: 30px;
      font-weight: bold;
      letter-spacing: 1px;
      transition: opacity 0.2s;
    }
    .hero a.cta:hover { opacity: 0.85; }

    .features {
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 60px 40px;
      flex-wrap: wrap;
      max-width: 1000px;
      margin: 0 auto;
    }
    .feature {
      background: #12121e;
      border: 1px solid #1e1e35;
      border-radius: 12px;
      padding: 30px;
      width: 280px;
      text-align: center;
    }
    .feature .icon { font-size: 2.5em; margin-bottom: 16px; }
    .feature h3 { margin-bottom: 10px; font-size: 1.1em; }
    .feature p { color: #888; font-size: 0.9em; line-height: 1.6; }

    .about {
      text-align: center;
      padding: 60px 40px;
      max-width: 700px;
      margin: 0 auto;
      border-top: 1px solid #1a1a2e;
    }
    .about h2 { margin-bottom: 20px; font-size: 1.6em; }
    .about p { color: #888; line-height: 1.8; }

    footer {
      text-align: center;
      padding: 30px;
      border-top: 1px solid #1a1a2e;
      color: #555;
      font-size: 0.85em;
    }
    footer a { color: #777; text-decoration: none; margin: 0 10px; }
    footer a:hover { color: #aaa; }
  </style>
</head>
<body>

<header>
  <div class="logo">KIYO KANSHI EDITS</div>
  <nav>
    <a href="https://www.tiktok.com/@kiyokanshiedits" target="_blank">TikTok</a>
    <a href="/privacy.html">Privacy</a>
    <a href="/terms.html">Terms</a>
  </nav>
</header>

<section class="hero">
  <h1>KIYO KANSHI EDITS</h1>
  <p>Daily anime edits crafted for the culture. JJK, Chainsaw Man, Solo Leveling, Bleach, Naruto and more — dropping every day.</p>
  <a class="cta" href="https://www.tiktok.com/@kiyokanshiedits" target="_blank">Follow on TikTok</a>
</section>

<section class="features">
  <div class="feature">
    <div class="icon">⚔️</div>
    <h3>Daily Edits</h3>
    <p>Three videos posted every day covering the best moments from the biggest anime series.</p>
  </div>
  <div class="feature">
    <div class="icon">🎵</div>
    <h3>Beat-Synced</h3>
    <p>Every cut lands on the beat. Edits are built around the music for maximum impact.</p>
  </div>
  <div class="feature">
    <div class="icon">🎨</div>
    <h3>Colour Graded</h3>
    <p>Custom colour grades for each anime series — JJK blues, Chainsaw Man reds, and more.</p>
  </div>
</section>

<section class="about">
  <h2>About</h2>
  <p>KiyoKanshiEdits is an anime content creation project dedicated to delivering high quality short-form edits daily. Videos are produced using our custom editing pipeline and published via TikTok's Content Posting API.</p>
</section>

<footer>
  <p>&copy; 2026 KiyoKanshiEdits. All rights reserved.</p>
  <a href="/privacy.html">Privacy Policy</a>
  <a href="/terms.html">Terms of Service</a>
  <a href="https://www.tiktok.com/@kiyokanshiedits" target="_blank">TikTok</a>
</footer>

</body>
</html>
