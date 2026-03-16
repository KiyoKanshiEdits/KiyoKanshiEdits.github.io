<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>KiyoKanshiEdits — Anime Content Tool</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: Arial, sans-serif; background: #0a0a0f; color: #fff; min-height: 100vh; }
    header { padding: 20px 40px; display: flex; justify-content: space-between; align-items: center; border-bottom: 1px solid #1a1a2e; }
    header .logo { font-size: 1.4em; font-weight: bold; letter-spacing: 2px; background: linear-gradient(90deg, #7b2fff, #ff3cac); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
    header nav a { color: #aaa; text-decoration: none; margin-left: 24px; font-size: 0.9em; }
    header nav a:hover { color: #fff; }
    .hero { text-align: center; padding: 100px 20px 60px; }
    .hero h1 { font-size: 2.8em; letter-spacing: 3px; background: linear-gradient(90deg, #7b2fff, #ff3cac, #ff6b35); -webkit-background-clip: text; -webkit-text-fill-color: transparent; margin-bottom: 20px; }
    .hero p { color: #aaa; font-size: 1.1em; max-width: 580px; margin: 0 auto 40px; line-height: 1.7; }
    .cta-group { display: flex; gap: 16px; justify-content: center; flex-wrap: wrap; }
    .hero a.cta { display: inline-block; padding: 14px 36px; background: linear-gradient(90deg, #7b2fff, #ff3cac); color: #fff; text-decoration: none; border-radius: 30px; font-weight: bold; }
    .hero a.cta-outline { display: inline-block; padding: 14px 36px; border: 1px solid #7b2fff; color: #7b2fff; text-decoration: none; border-radius: 30px; font-weight: bold; }
    .features { display: flex; justify-content: center; gap: 30px; padding: 60px 40px; flex-wrap: wrap; max-width: 1100px; margin: 0 auto; }
    .feature { background: #12121e; border: 1px solid #1e1e35; border-radius: 12px; padding: 30px; width: 240px; text-align: center; }
    .feature .icon { font-size: 2.5em; margin-bottom: 16px; }
    .feature h3 { margin-bottom: 10px; }
    .feature p { color: #888; font-size: 0.88em; line-height: 1.6; }
    .how-it-works { max-width: 750px; margin: 0 auto; padding: 60px 40px; border-top: 1px solid #1a1a2e; }
    .how-it-works h2 { text-align: center; margin-bottom: 40px; font-size: 1.6em; }
    .step { display: flex; gap: 20px; margin-bottom: 30px; align-items: flex-start; }
    .step .num { min-width: 36px; height: 36px; border-radius: 50%; background: linear-gradient(90deg, #7b2fff, #ff3cac); display: flex; align-items: center; justify-content: center; font-weight: bold; }
    .step .text h4 { margin-bottom: 6px; }
    .step .text p { color: #888; font-size: 0.9em; line-height: 1.6; }
    .about { text-align: center; padding: 60px 40px; max-width: 700px; margin: 0 auto; border-top: 1px solid #1a1a2e; }
    .about h2 { margin-bottom: 20px; font-size: 1.6em; }
    .about p { color: #888; line-height: 1.8; margin-bottom: 16px; }
    footer { text-align: center; padding: 30px; border-top: 1px solid #1a1a2e; color: #555; font-size: 0.85em; }
    footer a { color: #777; text-decoration: none; margin: 0 10px; }
  </style>
</head>
<body>

<header>
  <div class="logo">KIYO KANSHI EDITS</div>
  <nav>
    <a href="#how-it-works">How It Works</a>
    <a href="https://www.tiktok.com/@kiyokanshi" target="_blank">TikTok</a>
    <a href="/privacy.html">Privacy</a>
    <a href="/terms.html">Terms</a>
  </nav>
</header>

<section class="hero">
  <h1>ANIME CONTENT,<br>BUILT FOR TIKTOK</h1>
  <p>KiyoKanshiEdits is a content scheduling and publishing tool for anime creators. Connect your TikTok account and publish beat-synced anime edits on a consistent daily schedule.</p>
  <div class="cta-group">
    <a class="cta" href="https://www.tiktok.com/@kiyokanshi" target="_blank">See It In Action</a>
    <a class="cta-outline" href="#how-it-works">How It Works</a>
  </div>
</section>

<section class="features">
  <div class="feature">
    <div class="icon">🔗</div>
    <h3>TikTok Integration</h3>
    <p>Connect your TikTok account via OAuth and publish videos directly through TikTok's Content Posting API.</p>
  </div>
  <div class="feature">
    <div class="icon">📅</div>
    <h3>Scheduled Publishing</h3>
    <p>Set your posting schedule and let the tool handle publishing at peak engagement times automatically.</p>
  </div>
  <div class="feature">
    <div class="icon">🎵</div>
    <h3>Beat-Synced Edits</h3>
    <p>Every cut lands on the beat. Edits are automatically built around music for maximum viewer retention.</p>
  </div>
  <div class="feature">
    <div class="icon">🎨</div>
    <h3>Anime Colour Grades</h3>
    <p>Custom colour grades for JJK, Chainsaw Man, Bleach, Naruto and 15+ other series built in.</p>
  </div>
</section>

<section class="how-it-works" id="how-it-works">
  <h2>How It Works</h2>
  <div class="step">
    <div class="num">1</div>
    <div class="text">
      <h4>Connect Your TikTok Account</h4>
      <p>Authenticate via TikTok's OAuth flow. The tool uses TikTok's official Content Posting API — your credentials are never stored on our servers.</p>
    </div>
  </div>
  <div class="step">
    <div class="num">2</div>
    <div class="text">
      <h4>Generate Your Edit</h4>
      <p>The editing engine automatically builds a beat-synced vertical video from your selected anime clips and music, with colour grading and watermark applied.</p>
    </div>
  </div>
  <div class="step">
    <div class="num">3</div>
    <div class="text">
      <h4>Review and Approve</h4>
      <p>Preview the finished video before it goes live. Approve it for publishing or generate a new version.</p>
    </div>
  </div>
  <div class="step">
    <div class="num">4</div>
    <div class="text">
      <h4>Auto-Publish to TikTok</h4>
      <p>Approved videos are published directly to your TikTok account via the Content Posting API on your chosen schedule.</p>
    </div>
  </div>
</section>

<section class="about">
  <h2>About</h2>
  <p>KiyoKanshiEdits is an anime content creation and publishing tool built for TikTok creators who want to grow their channels with consistent, high-quality edits.</p>
  <p>The tool handles the full workflow — from editing and colour grading to scheduling and publishing — so creators can focus on content strategy rather than manual production.</p>
  <p>Built by anime fans, for anime fans.</p>
</section>

<footer>
  <p>&copy; 2026 KiyoKanshiEdits. All rights reserved.</p>
  <a href="/privacy.html">Privacy Policy</a>
  <a href="/terms.html">Terms of Service</a>
  <a href="https://www.tiktok.com/@kiyokanshi" target="_blank">TikTok</a>
</footer>

</body>
</html>
