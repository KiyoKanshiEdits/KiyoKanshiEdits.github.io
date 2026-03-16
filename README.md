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
    .btn { display: inline-block; padding: 14px 36px; border-radius: 30px; font-weight: bold; letter-spacing: 1px; cursor: pointer; font-size: 1em; border: none; }
    .btn-primary { background: linear-gradient(90deg, #7b2fff, #ff3cac); color: #fff; }
    .btn-outline { background: transparent; border: 1px solid #7b2fff; color: #7b2fff; }
    .btn:hover { opacity: 0.85; }

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

    /* Connect section */
    .connect-section { text-align: center; padding: 60px 40px; border-top: 1px solid #1a1a2e; }
    .connect-section h2 { margin-bottom: 16px; font-size: 1.6em; }
    .connect-section p { color: #aaa; margin-bottom: 32px; max-width: 480px; margin-left: auto; margin-right: auto; line-height: 1.7; }
    .connect-box { background: #12121e; border: 1px solid #1e1e35; border-radius: 16px; max-width: 420px; margin: 0 auto; padding: 40px 30px; }
    .connect-box h3 { margin-bottom: 10px; }
    .connect-box p { color: #888; font-size: 0.9em; margin-bottom: 24px; line-height: 1.6; }
    .tiktok-btn { display: flex; align-items: center; justify-content: center; gap: 10px; width: 100%; padding: 14px; background: #000; color: #fff; border: none; border-radius: 8px; font-size: 1em; font-weight: bold; cursor: pointer; margin-bottom: 12px; }
    .tiktok-btn:hover { background: #111; }
    .tiktok-btn svg { width: 20px; height: 20px; fill: #fff; }
    .or-divider { color: #555; font-size: 0.85em; margin: 16px 0; }
    .example-link { color: #7b2fff; text-decoration: none; font-size: 0.9em; }
    .example-link:hover { text-decoration: underline; }

    /* Modal */
    .modal-overlay { display: none; position: fixed; inset: 0; background: rgba(0,0,0,0.75); z-index: 100; align-items: center; justify-content: center; }
    .modal-overlay.active { display: flex; }
    .modal { background: #12121e; border: 1px solid #1e1e35; border-radius: 16px; padding: 40px; max-width: 420px; width: 90%; text-align: center; position: relative; }
    .modal h3 { margin-bottom: 12px; font-size: 1.3em; }
    .modal p { color: #aaa; line-height: 1.7; margin-bottom: 24px; font-size: 0.95em; }
    .modal input { width: 100%; padding: 12px 16px; background: #0a0a0f; border: 1px solid #2a2a45; border-radius: 8px; color: #fff; font-size: 0.95em; margin-bottom: 12px; }
    .modal input::placeholder { color: #555; }
    .modal .close-btn { position: absolute; top: 16px; right: 20px; background: none; border: none; color: #666; font-size: 1.4em; cursor: pointer; }
    .modal .close-btn:hover { color: #fff; }
    .badge { display: inline-block; background: linear-gradient(90deg, #7b2fff33, #ff3cac33); border: 1px solid #7b2fff55; border-radius: 20px; padding: 4px 14px; font-size: 0.8em; color: #cc88ff; margin-bottom: 16px; }

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
    <a href="#connect">Get Access</a>
    <a href="https://www.tiktok.com/@kiyokanshi" target="_blank">TikTok</a>
    <a href="/privacy.html">Privacy</a>
    <a href="/terms.html">Terms</a>
  </nav>
</header>

<section class="hero">
  <h1>ANIME CONTENT,<br>BUILT FOR TIKTOK</h1>
  <p>KiyoKanshiEdits is a content scheduling and publishing tool for anime creators. Connect your TikTok account and publish beat-synced anime edits on a consistent daily schedule.</p>
  <div class="cta-group">
    <button class="btn btn-primary" onclick="openModal()">Connect TikTok</button>
    <a class="btn btn-outline" href="https://www.tiktok.com/@kiyokanshi" target="_blank">View Example</a>
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

<section class="connect-section" id="connect">
  <h2>Get Early Access</h2>
  <p>Creator access is currently in limited beta. Connect your TikTok account or join the waitlist to be notified when access opens.</p>
  <div class="connect-box">
    <div class="badge">Beta</div>
    <h3>Connect Your Account</h3>
    <p>Authenticate with TikTok to link your creator account and start publishing anime edits automatically.</p>
    <button class="tiktok-btn" onclick="openModal()">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.59 6.69a4.83 4.83 0 01-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 01-2.88 2.5 2.89 2.89 0 01-2.89-2.89 2.89 2.89 0 012.89-2.89c.28 0 .54.04.79.1V9.01a6.33 6.33 0 00-.79-.05 6.34 6.34 0 00-6.34 6.34 6.34 6.34 0 006.34 6.34 6.34 6.34 0 006.33-6.34V8.69a8.18 8.18 0 004.79 1.54V6.78a4.85 4.85 0 01-1.02-.09z"/></svg>
      Continue with TikTok
    </button>
    <div class="or-divider">or</div>
    <a class="example-link" href="https://www.tiktok.com/@kiyokanshi" target="_blank">View example content on TikTok →</a>
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

<!-- Waitlist Modal -->
<div class="modal-overlay" id="modalOverlay">
  <div class="modal">
    <button class="close-btn" onclick="closeModal()">×</button>
    <div class="badge">Limited Beta</div>
    <h3>Join the Waitlist</h3>
    <p>Creator access is currently limited while we finalise TikTok API integration. Enter your email and we'll notify you as soon as access opens.</p>
    <input type="email" placeholder="your@email.com" id="waitlistEmail" />
    <button class="btn btn-primary" style="width:100%;justify-content:center;" onclick="submitWaitlist()">Notify Me</button>
  </div>
</div>

<script>
  function openModal() {
    document.getElementById('modalOverlay').classList.add('active');
  }
  function closeModal() {
    document.getElementById('modalOverlay').classList.remove('active');
  }
  function submitWaitlist() {
    const email = document.getElementById('waitlistEmail').value;
    if (!email || !email.includes('@')) {
      alert('Please enter a valid email address.');
      return;
    }
    document.querySelector('.modal h3').textContent = "You're on the list!";
    document.querySelector('.modal p').textContent = "We'll email you at " + email + " when creator access opens.";
    document.querySelector('.modal input').style.display = 'none';
    document.querySelector('.modal .btn').style.display = 'none';
  }
  document.getElementById('modalOverlay').addEventListener('click', function(e) {
    if (e.target === this) closeModal();
  });
</script>

</body>
</html>
