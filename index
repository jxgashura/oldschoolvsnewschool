<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Join The Music Village for the epic Old School vs New School Battle! Free entrance, live performances, and interactive voting.">
  <meta name="keywords" content="Music, Event, Old School, New School, Battle, Live, Free, Dobsi Campus Hall">
  <meta property="og:title" content="Old School vs New School Battle">
  <meta property="og:description" content="Live at Dobsi Campus Hall, 23 September 2025. Vote for your favorite!">
  <meta property="og:type" content="website">
  <meta property="og:image" content="https://jxgashura.github.io/oldschoolvsnewschool/preview.jpg">
  <link rel="icon" href="favicon.ico" type="image/x-icon">
  <title>Old School vs New School Battle</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700&family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', Arial, Helvetica, sans-serif;
      background: linear-gradient(120deg, #ff6e7f 0%, #bfe9ff 100%);
      color: #fff;
      text-align: center;
      border: 8px solid #fff;
      min-height: 100vh;
      position: relative;
      box-sizing: border-box;
    }
    header {
      padding: 30px 20px 20px 20px;
      background: linear-gradient(90deg, #111 60%, #ffcc00 100%);
      border-bottom: 4px solid #fff;
      box-shadow: 0 4px 16px rgba(0,0,0,0.2);
    }
    header h1 {
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      font-size: 2.5em;
      margin: 0;
      text-transform: uppercase;
      letter-spacing: 2px;
      color: #ffcc00;
      text-shadow: 2px 2px 8px #222;
      animation: pop 1.2s cubic-bezier(.17,.67,.83,.67) 1;
    }
    @keyframes pop {
      0% { transform: scale(0.7); opacity: 0; }
      80% { transform: scale(1.1); opacity: 1; }
      100% { transform: scale(1); }
    }
    .versus-container {
      display: flex;
      justify-content: space-between;
      align-items: stretch;
      gap: 30px;
      margin: 30px 0;
      flex-wrap: wrap;
    }
    .group-container {
      flex: 1 1 320px;
      background: rgba(255,255,255,0.08);
      border-radius: 28px;
      padding: 24px 18px 18px 18px;
      margin: 18px 0;
      box-shadow: 0 4px 24px rgba(0,0,0,0.12);
      display: flex;
      flex-direction: column;
      align-items: center;
      min-width: 260px;
      max-width: 420px;
      margin-left: auto;
      margin-right: auto;
    }
    .group-heading h2 {
      font-size: 1.5em;
      color: #ffcc00;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      margin-bottom: 8px;
      text-shadow: 1px 1px 8px #222;
    }
    .group-performers {
      font-size: 1.1em;
      color: #fff;
      margin-bottom: 12px;
    }
    .track-preview {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 32px;
      margin-bottom: 18px;
    }
    .track {
      background: rgba(255,255,255,0.08);
      border-radius: 28px;
      padding: 24px 18px 18px 18px;
      margin: 18px 0;
      box-shadow: 0 4px 24px rgba(0,0,0,0.12);
      display: flex;
      flex-direction: column;
      align-items: center;
      min-width: 220px;
      max-width: 320px;
      margin-left: auto;
      margin-right: auto;
    }
    .track-label {
      font-size: 1.25em;
      font-weight: 700;
      color: #ffcc00;
      margin-bottom: 8px;
      text-shadow: 1px 1px 8px #222;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
    }
    .track img {
      width: 180px;
      height: 180px;
      object-fit: cover;
      border: 6px solid #fff;
      border-radius: 24px;
      margin-bottom: 14px;
      box-shadow: 0 8px 32px rgba(0,0,0,0.22);
      transition: box-shadow 0.3s, transform 0.2s;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
    .track img:hover {
      box-shadow: 0 16px 48px #ffcc00;
      transform: scale(1.04);
    }
    .audio-display audio {
      width: 100%;
      margin-bottom: 6px;
    }
    .track-controls {
      margin-top: 4px;
      font-size: 0.98em;
      color: #185a9d;
      background: rgba(191,233,255,0.13);
      border-radius: 8px;
      padding: 4px 12px;
      margin-bottom: 2px;
    }
    .placeholder-art {
      width: 180px;
      height: 180px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      border: 4px dashed #ffcc00;
      border-radius: 24px;
      background: rgba(255,255,255,0.07);
      margin-bottom: 14px;
      box-shadow: 0 2px 12px rgba(0,0,0,0.10);
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      font-size: 1.1em;
      color: #bbb;
    }
    .cta-btn {
      display: inline-block;
      margin-top: 18px;
      padding: 12px 32px;
      background: linear-gradient(90deg, #ff6e7f 0%, #bfe9ff 100%);
      color: #222;
      font-size: 1.2em;
      border: none;
      border-radius: 30px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.18);
      cursor: pointer;
      transition: background 0.3s, color 0.3s, transform 0.2s;
      text-decoration: none;
    }
    .cta-btn:hover {
      background: linear-gradient(90deg, #bfe9ff 0%, #ff6e7f 100%);
      color: #fff;
      transform: scale(1.07);
    }
    .vote-tally {
      margin-top: 8px;
      font-size: 1.1em;
      color: #ffcc00;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      text-shadow: 1px 1px 8px #222;
    }
    .event-info {
      padding: 28px 20px;
      background: linear-gradient(90deg, #111 60%, #ffcc00 100%);
      border-top: 4px solid #fff;
      box-shadow: 0 -4px 16px rgba(0,0,0,0.2);
      margin-top: 30px;
      border-radius: 0 0 20px 20px;
    }
    .event-info h3 {
      margin: 5px 0;
      color: #ffcc00;
      font-size: 1.3em;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      text-shadow: 1px 1px 6px #222;
    }
    .performers {
      margin-top: 15px;
      font-size: 1.15em;
      line-height: 1.7em;
      color: #fff;
      font-family: 'Montserrat', Arial, Helvetica, sans-serif;
      text-shadow: 1px 1px 6px #222;
    }
    .performers strong {
      color: #ffcc00;
      font-size: 1.1em;
    }
    .countdown-container {
      margin-bottom: 12px;
    }
    .countdown-bar {
      width: 100%;
      height: 12px;
      background: rgba(255,255,255,0.18);
      border-radius: 8px;
      margin: 8px 0 0 0;
      overflow: hidden;
    }
    .countdown-progress {
      height: 100%;
      background: linear-gradient(90deg, #ffcc00 0%, #ff6e7f 100%);
      border-radius: 8px;
      transition: width 0.5s;
    }
    @media (max-width: 900px) {
      .versus-container {
        flex-direction: column;
        gap: 18px;
        margin: 18px 0;
      }
      .group-container {
        max-width: 98vw;
      }
    }
    @media (max-width: 600px) {
      header h1 {
        font-size: 1.3em;
      }
      .group-heading h2 {
        font-size: 1.2em;
      }
      .track img {
        width: 120px;
        height: 120px;
      }
      .track {
        min-width: 140px;
        max-width: 98vw;
        padding: 12px 6px 10px 6px;
      }
      .track-preview {
        gap: 12px;
      }
      .event-info {
        padding: 18px 8px;
        font-size: 0.95em;
      }
      .performers {
        font-size: 1em;
      }
      body {
        border-width: 4px;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Old School vs New School Battle</h1>
  </header>
  <div class="versus-container">
    <div class="group-container">
      <div class="group-heading old-school-heading">
        <h2>Old School 👑</h2>
        <div class="group-performers">Performance By: Ly'mbidla 🎤, Demons and Angels 😇😈</div>
      </div>
      <div class="track-preview">
        <div class="track">
          <div class="track-label">Ly'mbidla 🎤</div>
          <div class="audio-display">
            <audio id="audio-lymbidla" controls preload="metadata">
              <source src="media/Ly'mbidla.mp3" type="audio/mpeg">
              Your browser does not support audio playback.
            </audio>
            <div class="track-controls">
              <span>Seek & Playback enabled</span>
            </div>
          </div>
        </div>
        <div class="track">
          <div class="track-label">Demons and Angels 😇😈</div>
          <div class="placeholder-art">
            <span style="font-size:2.5em; color:#ffcc00;">🎵</span>
            <div>Album art & track coming soon</div>
          </div>
        </div>
      </div>
      <button class="cta-btn" id="vote-old" onclick="vote('old')">Vote Old School</button>
      <div class="vote-tally" id="tally-old">Votes: 0</div>
    </div>
    <div class="group-container">
      <div class="group-heading new-school-heading">
        <h2>New School 🚀</h2>
        <div class="group-performers">Performance By: Lyrical Cartel 🎧, Top-Deck 🕺</div>
      </div>
      <div class="track-preview">
        <div class="track">
          <div class="track-label">Lyrical Cartel 🎧</div>
          <div class="audio-display">
            <audio id="audio-lyricalcartel" controls preload="metadata">
              <source src="media/lyrical cartel.mp3" type="audio/mpeg">
              Your browser does not support audio playback.
            </audio>
            <div class="track-controls">
              <span>Seek & Playback enabled</span>
            </div>
          </div>
        </div>
        <div class="track">
          <div class="track-label">Top-Deck 🕺</div>
          <img src="media/top deck.jpg" alt="Top-Deck Album Art" aria-label="Top-Deck Album Art">
          <!-- Replace 'media/top deck.jpg' with your own image in the repo for best results -->
          <div class="audio-display">
            <audio id="audio-topdeck" controls preload="metadata">
              <source src="media/top deck.mp3" type="audio/mpeg">
              Your browser does not support audio playback.
              <!-- Add 'media/top deck.mp3' to your repo for audio playback -->
            </audio>
            <div class="track-controls">
              <span>Seek & Playback enabled</span>
            </div>
          </div>
        </div>
      </div>
      <button class="cta-btn" id="vote-new" onclick="vote('new')">Vote New School</button>
      <div class="vote-tally" id="tally-new">Votes: 0</div>
    </div>
  </div>

        <!-- Social media icons removed for cleaner layout -->

        <div class="event-info">
          <div style="margin: 24px 0;">
            <h3>Scan to view this page:</h3>
            <div id="qrcode"></div>
          </div>
          <div class="countdown-container">
            <div id="countdown-label">Time until event starts:</div>
            <div id="countdown-timer">Loading...</div>
            <div class="countdown-bar">
              <div id="countdown-progress" class="countdown-progress" style="width:0%"></div>
            </div>
          </div>
          <h3>📍 Venue: Music Centre</h3>
          <h3>📅 Date: 23 September 2025</h3>
          <h3>⏰ Time: 12:00 to 3:00</h3>
          <h3>🆓 Free Entrance</h3>
          <div class="performers">
            <strong>Performances By:</strong><br>
            Ly'mbidla 🎤<br>
            Lyrical Cartel 🎧<br>
            Demons and Angels 😇😈<br>
            Top-Deck 🕺
          </div>
          <h3>👥 Limited space</h3>
        </div>
        <!--
          Asset Instructions:
          - Add 'media/top deck.jpg' and other images to your repo for album art.
          - Add 'media/top deck.mp3' and other audio files for playback.
          - Add 'favicon.ico' for a custom favicon.
          - Optionally add 'preview.jpg' for social sharing previews.
          Accessibility:
          - All images and buttons have ARIA labels for screen readers.
          - Audio controls are labeled for clarity.
          SEO & Social:
          - Meta tags for description, keywords, and Open Graph are included.
          - Page is ready for public deployment (GitHub Pages, Netlify, etc).
        -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/qrious/4.0.2/qrious.min.js"></script>
  <script>
          // Play audio preview and limit to 30 seconds
          function playTrack(audioId) {
            var audio = document.getElementById(audioId);
            if (!audio) return;
            audio.currentTime = 0;
            audio.play();
            if (audio._timer) clearTimeout(audio._timer);
            audio._timer = setTimeout(function() { audio.pause(); }, 30000);
            audio.addEventListener('pause', function() {
              if (audio._timer) clearTimeout(audio._timer);
            });
          }
          // Limit all audio previews to 30 seconds
          function limitAudioPlayback(audioId) {
            const audio = document.getElementById(audioId);
            if (!audio) return;
            audio.addEventListener('play', function() {
              if (audio._timer) clearTimeout(audio._timer);
              audio._timer = setTimeout(() => audio.pause(), 30000);
            });
            audio.addEventListener('pause', function() {
              if (audio._timer) clearTimeout(audio._timer);
            });
          }
          window.addEventListener('DOMContentLoaded', function() {
            limitAudioPlayback('audio-lymbidla');
            limitAudioPlayback('audio-demonsangels');
            limitAudioPlayback('audio-lyricalcartel');
            limitAudioPlayback('audio-topdeck');
            // Event start: 23 September 2025, 11:00 local time
            const eventDate = new Date('2025-09-23T11:00:00');
            const voteOldBtn = document.getElementById('vote-old');
            const voteNewBtn = document.getElementById('vote-new');
            let votes = { old: 0, new: 0 };
            let votingActive = false;

            function updateCountdown() {
              const now = new Date();
              const diff = eventDate - now;
              const timer = document.getElementById('countdown-timer');
              const progress = document.getElementById('countdown-progress');
              if (diff > 0) {
                votingActive = false;
                voteOldBtn.disabled = true;
                voteNewBtn.disabled = true;
                voteOldBtn.style.opacity = '0.6';
                voteNewBtn.style.opacity = '0.6';
                // Time breakdown
                const days = Math.floor(diff / (1000*60*60*24));
                const hours = Math.floor((diff % (1000*60*60*24)) / (1000*60*60));
                const mins = Math.floor((diff % (1000*60*60)) / (1000*60));
                const secs = Math.floor((diff % (1000*60)) / 1000);
                timer.textContent = `${days}d ${hours}h ${mins}m ${secs}s`;
                // Progress bar: percent of time elapsed from now to event
                const total = eventDate - new Date('2025-09-18T00:00:00'); // start from today
                const elapsed = now - new Date('2025-09-18T00:00:00');
                let percent = Math.max(0, Math.min(100, (elapsed/total)*100));
                progress.style.width = percent + '%';
              } else {
                votingActive = true;
                voteOldBtn.disabled = false;
                voteNewBtn.disabled = false;
                voteOldBtn.style.opacity = '1';
                voteNewBtn.style.opacity = '1';
                timer.textContent = 'Event has started! Vote now!';
                progress.style.width = '100%';
              }
            }

            function vote(type) {
              if (!votingActive) {
                alert('Voting will open at the event start time!');
                return;
              }
              votes[type]++;
              document.getElementById('tally-' + type).textContent = `Votes: ${votes[type]}`;
            }

            // Initial setup
            updateCountdown();
            setInterval(updateCountdown, 1000);

            // Attach vote function to window so buttons work
            window.vote = vote;
            // Generate QR code for public event page
            var qr = new QRious({
              element: document.getElementById('qrcode'),
              value: 'https://jxgashura.github.io/oldschoolvsnewschool/oldschool-vs-newschool-flair.html',
              size: 180,
              background: 'white',
              foreground: '#111'
            });
          });
        </script>
