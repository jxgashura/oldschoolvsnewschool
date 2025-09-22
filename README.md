# oldschoolvsnewschool
Assignment.

Skip to content
Navigation Menu
jxgashura
oldschoolvsnewschool

Type / to search
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
Settings
Files
Go to file
t
README.md
oldschool-vs-newschool-flair (1).html
oldschoolvsnewschool
/oldschool-vs-newschool-flair (1).html
 

Code

Blame
435 lines (435 loc) · 12.9 KB
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
      overflow-x: hidden;
    }
    header {
      padding: 30px 20px 20px 20px;
      background: linear-gradient(90deg, #111 60%, #ffcc00 100%);
      border-bottom: 4px solid #fff;
      box-shadow: 0 4px 16px rgba(0,0,0,0.2);
      position: relative;
    }
    header h1 {
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      font-size: 2.7em;
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
    .neon {
      color: #fff;
      text-shadow: 0 0 8px #00ffe7, 0 0 24px #00ffe7, 0 0 48px #ff00cc;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      letter-spacing: 2px;
      font-size: 1.1em;
      animation: neonPulse 2s infinite alternate;
    }
    @keyframes neonPulse {
      0% { text-shadow: 0 0 8px #00ffe7, 0 0 24px #00ffe7, 0 0 48px #ff00cc; }
      100% { text-shadow: 0 0 16px #00ffe7, 0 0 32px #00ffe7, 0 0 64px #ff00cc; }
    }
    .versus-container {
      display: flex;
      justify-content: space-between;
      align-items: stretch;
      height: 60vh;
      margin: 30px 0;
      gap: 30px;
    }
    @media (max-width: 900px) {
      .versus-container {
        flex-direction: column;
        height: auto;
        gap: 18px;
        margin: 18px 0;
      }
      .side {
        margin-bottom: 0;
      }
    }
    @media (max-width: 600px) {
      header h1 {
        font-size: 1.3em;
      }
      .side h2 {
        font-size: 1.2em;
      }
      .side img {
        width: 120px;
        height: 120px;
      }
      audio {
        width: 100%;
      }
      .cta-btn {
        font-size: 1em;
        padding: 10px 18px;
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
      .social-icons a {
        font-size: 1.5em;
        padding: 6px;
      }
    }
    .side {
      flex: 1;
      padding: 30px 20px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      border-radius: 20px;
      box-shadow: 0 8px 32px rgba(0,0,0,0.18);
      transition: transform 0.3s, box-shadow 0.3s;
      position: relative;
    }
    .side:hover {
      transform: scale(1.04);
      box-shadow: 0 12px 40px rgba(0,0,0,0.28);
    }
    .old-school {
      background: linear-gradient(135deg, #ffb347 0%, #ffcc33 100%);
      color: #222;
      border: 2px solid #ffcc00;
      box-shadow: 0 0 24px #ffcc00;
    }
    .new-school {
      background: linear-gradient(135deg, #43cea2 0%, #185a9d 100%);
      color: #fff;
      border: 2px solid #43cea2;
      box-shadow: 0 0 24px #43cea2;
    }
    .side h2 {
      font-size: 2em;
      margin-bottom: 10px;
      color: #fff;
      text-transform: uppercase;
      letter-spacing: 1px;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      text-shadow: 1px 1px 6px #222;
    }
    .side img {
      width: 180px;
      height: 180px;
      object-fit: cover;
      border: 4px solid #fff;
      border-radius: 18px;
      margin-bottom: 10px;
      box-shadow: 0 4px 16px rgba(0,0,0,0.18);
      transition: box-shadow 0.3s;
    }
    .side img:hover {
      box-shadow: 0 8px 32px #ffcc00;
    }
    audio {
      width: 80%;
      outline: none;
      margin-bottom: 10px;
    }
    .cta-btn {
      display: inline-block;
      margin-top: 18px;
      padding: 12px 32px;
      background: linear-gradient(90deg, #ff6e7f 0%, #bfe9ff 100%);
      color: #222;
      font-size: 1.2em;
      font-weight: bold;
      border: none;
      border-radius: 30px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.18);
      cursor: pointer;
      transition: background 0.3s, color 0.3s, transform 0.2s;
      text-decoration: none;
      position: relative;
      overflow: hidden;
    }
    .cta-btn:active {
      animation: btnPulse 0.3s;
    }
    @keyframes btnPulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.12); }
      100% { transform: scale(1); }
    }
    .cta-btn:hover {
      background: linear-gradient(90deg, #bfe9ff 0%, #ff6e7f 100%);
      color: #fff;
      transform: scale(1.07);
    }
    .vote-tally {
      margin-top: 10px;
      font-size: 1.1em;
      font-weight: bold;
      color: #fff;
      text-shadow: 0 0 8px #00ffe7, 0 0 24px #ff00cc;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
    }
    .confetti {
      position: absolute;
      left: 50%;
      top: 50%;
      pointer-events: none;
      z-index: 999;
      width: 0;
      height: 0;
    }
    .event-info {
      padding: 28px 20px;
      background: linear-gradient(90deg, #111 60%, #ffcc00 100%);
      border-top: 4px solid #fff;
      box-shadow: 0 -4px 16px rgba(0,0,0,0.2);
      margin-top: 30px;
      border-radius: 0 0 20px 20px;
      position: relative;
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
      margin-bottom: 18px;
      animation: pulse 1.5s infinite alternate;
    }
    @keyframes pulse {
      0% { box-shadow: 0 0 8px #ffcc00; }
      100% { box-shadow: 0 0 24px #ffcc00; }
    }
    #countdown-timer {
      font-size: 1.3em;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      margin: 8px 0;
      color: #fff;
      text-shadow: 0 0 8px #00ffe7, 0 0 24px #ff00cc;
    }
    .countdown-bar {
      width: 80%;
      height: 12px;
      background: #fff2;
      border-radius: 8px;
      margin: 10px auto 0 auto;
      overflow: hidden;
      box-shadow: 0 2px 8px #ffcc00;
    }
    .countdown-progress {
      height: 100%;
      background: linear-gradient(90deg, #ffcc00 0%, #ff6e7f 100%);
      border-radius: 8px;
      transition: width 0.5s;
    }
    .social-icons {
      margin-top: 18px;
      display: flex;
      gap: 18px;
      justify-content: center;
    }
    .social-icons a {
      color: #fff;
      font-size: 2em;
      transition: color 0.2s;
      text-decoration: none;
    }
    .social-icons a:hover {
      color: #ffcc00;
    }
    footer {
      margin-top: 40px;
      padding: 18px 0;
      background: linear-gradient(90deg, #111 60%, #ffcc00 100%);
      color: #fff;
      font-family: 'Orbitron', Arial, Helvetica, sans-serif;
      font-size: 1em;
      border-radius: 0 0 20px 20px;
      box-shadow: 0 -2px 8px rgba(0,0,0,0.18);
    }
  </style>
</head>
<body>
  <header>
    <h1>🎶 The Music Village Presents:<br>Old School vs New School <span class="neon">🔥</span><br>Battle of the Ages</h1>
  </header>
  <div class="versus-container">
    <div class="side old-school">
      <h2>Old School 👑</h2>
      <img src="oldschool-art.jpg" alt="Old School Album Art">
      <audio controls>
        <source src="oldschool-snippet.mp3" type="audio/mpeg">
        Your browser does not support audio playback.
      </audio>
      <button class="cta-btn" id="vote-old" onclick="vote('old')">Vote Old School</button>
      <div class="vote-tally" id="tally-old">Votes: 0</div>
      <canvas class="confetti" id="confetti-old"></canvas>
    </div>
    <div class="side new-school">
      <h2>New School 🚀</h2>
      <img src="newschool-art.jpg" alt="New School Album Art">
      <audio controls>
        <source src="newschool-snippet.mp3" type="audio/mpeg">
        Your browser does not support audio playback.
      </audio>
      <button class="cta-btn" id="vote-new" onclick="vote('new')">Vote New School</button>
      <div class="vote-tally" id="tally-new">Votes: 0</div>
      <canvas class="confetti" id="confetti-new"></canvas>
    </div>
  </div>
  <div class="event-info">
    <div class="countdown-container">
      <div id="countdown-label">Time until event starts:</div>
      <div id="countdown-timer">Loading...</div>
      <div class="countdown-bar">
        <div id="countdown-progress" class="countdown-progress" style="width:0%"></div>
      </div>
    </div>
    <h3>📍 Venue: Dobsi Campus Hall</h3>
    <h3>📅 Date: 23 September 2025</h3>
    <h3>⏰ Time: 11:00</h3>
    <h3>🆓 Free Entrance</h3>
    <div class="performers">
      <strong>Performances By:</strong><br>
      Ly'mbidla 🎤<br>
      Lyrical Cartel 🎧<br>
      Demons and Angels 😇😈<br>
      Top-Deck 🕺
    </div>
    <div class="social-icons">
      <a href="#" title="Share on Instagram"><span>📸</span></a>
      <a href="#" title="Share on TikTok"><span>🎵</span></a>
      <a href="#" title="Share on X"><span>🐦</span></a>
    </div>
  </div>
  <footer>
  &copy; 2025 The Music Village. Stay tuned for more epic showcases of talent!
  </footer>
  <script>
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
      launchConfetti(type);
      playVoteSound();
    }
    // Confetti effect
    function launchConfetti(type) {
      const canvas = document.getElementById('confetti-' + type);
      canvas.width = 200;
      canvas.height = 120;
      const ctx = canvas.getContext('2d');
      ctx.clearRect(0,0,canvas.width,canvas.height);
      for(let i=0;i<30;i++){
        ctx.save();
        ctx.beginPath();
        ctx.arc(Math.random()*canvas.width,Math.random()*canvas.height,Math.random()*8+4,0,2*Math.PI);
        ctx.fillStyle = `hsl(${Math.random()*360},100%,60%)`;
        ctx.globalAlpha = 0.7;
        ctx.fill();
        ctx.restore();
      }
      setTimeout(()=>ctx.clearRect(0,0,canvas.width,canvas.height),700);
    }
    // Fun vote sound
    function playVoteSound() {
      const ctx = new(window.AudioContext||window.webkitAudioContext)();
      const o = ctx.createOscillator();
      const g = ctx.createGain();
      o.type = 'triangle';
      o.frequency.value = 440 + Math.random()*220;
      g.gain.value = 0.15;
      o.connect(g);
      g.connect(ctx.destination);
      o.start();
      o.stop(ctx.currentTime+0.18);
    }
    // Initial setup
    updateCountdown();
    setInterval(updateCountdown, 1000);
  </script>
</body>
</html>
oldschoolvsnewschool/oldschool-vs-newschool-flair (1).html at main · jxgashura/oldschoolvsnewschool 
