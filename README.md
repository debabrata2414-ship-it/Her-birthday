
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday Tuuaa Raniii ❤️❤️😘</title>

  <!-- ✅ Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

  <style>
    /* Reset */
    body, html {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow-x: hidden;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #ffd6e8, #fff0f5);
      position: relative;
    }

    /* Canvas full screen behind */
    #loveCanvas {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      pointer-events: none;
      z-index: 0;
      mix-blend-mode: screen; /* softly blend hearts with background */
    }

    /* Container on top */
    .container {
      position: relative;
      z-index: 10;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 30px;
    }

    .click-box {
      background-color: #ff69b4;
      color: white;
      padding: 20px 40px;
      font-size: 24px;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.3s ease;
      margin-top: 100px;
      z-index: 10;
      position: relative;
      box-shadow: 0 4px 12px rgba(255,20,147,0.6);
    }

    .click-box:hover {
      background-color: #ff1493;
      box-shadow: 0 6px 18px rgba(255,20,147,0.9);
    }

    .cake-section, .message-section, .gift-section, .gallery-section, .slideshow-section {
      display: none;
      flex-direction: column;
      align-items: center;
      animation: fadeIn 2s ease forwards;
      z-index: 10;
      position: relative;
    }

    .cake {
      font-size: 50px;
      margin: 40px 0 10px;
      text-shadow: 0 0 12px #ff69b4;
      color: #d81b60;
    }

    .name {
      font-size: 30px;
      font-weight: bold;
      color: #ff1493;
      margin-bottom: 20px;
      text-shadow: 0 0 8px #ff1493;
    }

    .message {
      max-width: 800px;
      font-size: 26px;
      line-height: 1.6;
      background: rgba(255, 255, 255, 0.85);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(255, 105, 180, 0.4);
      color: #900048;
    }

    .heart-box {
      font-size: 100px;
      cursor: pointer;
      animation: pulse 1.5s infinite;
      color: #ff007f;
      text-shadow: 0 0 15px #ff007f;
      z-index: 10;
      position: relative;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.15); }
      100% { transform: scale(1); }
    }

    .firework {
      position: fixed;
      width: 10px;
      height: 10px;
      background: radial-gradient(circle, #ff69b4, #fff0f5);
      border-radius: 50%;
      animation: explode 1.2s ease-out forwards;
      box-shadow: 0 0 20px #fff5fa, 0 0 30px #ff69b4;
    }

    @keyframes explode {
      0% { transform: scale(1); opacity: 1; }
      100% { transform: scale(25); opacity: 0; }
    }

    .slideshow-section img {
      width: 90vw;
      max-width: 600px;
      border-radius: 15px;
      box-shadow: 0 0 20px rgba(255, 105, 180, 0.5);
      display: none;
      animation: fadeIn 1s ease forwards;
      position: relative;
      z-index: 10;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .music-disc {
      position: fixed;
      top: 20px;
      left: 20px;
      width: 80px;
      height: 80px;
      border-radius: 50%;
      background: url('img3.jpg') no-repeat center/cover;
      border: 3px solid #ff69b4;
      animation: spin 5s linear infinite;
      box-shadow: 0 0 20px rgba(255, 192, 203, 0.7);
      z-index: 10;
    }

    /* Zoom Out Label with Arrow */
    .zoom-label {
      position: fixed;
      top: 110px;
      left: 20px;
      font-family: 'Dancing Script', cursive;
      font-size: 36px;
      color: #ff1493;
      font-weight: bold;
      text-shadow: 1px 1px 4px #fff;
      z-index: 10;
    }

    .arrow {
      display: inline-block;
      margin-left: 12px;
      font-size: 42px;
      color: #ff1493;
      font-weight: bold;
      animation: arrowFloat 2s ease-in-out infinite;
      transform: translateY(4px);
      text-shadow: 0 0 8px rgba(255, 105, 180, 0.5);
    }

    @keyframes arrowFloat {
      0% { transform: translateX(0) translateY(4px); opacity: 1; }
      50% { transform: translateX(8px) translateY(4px); opacity: 0.7; }
      100% { transform: translateX(0) translateY(4px); opacity: 1; }
    }

    @keyframes spin {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }

    /* Star and Heart backgrounds - keep behind */
    .stars, .hearts {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: -1;
    }

    .stars {
      background-image: radial-gradient(#ffffff33 1px, transparent 1px);
      background-size: 30px 30px;
    }

    .hearts::before {
      content: '💖💞💕💓💘';
      font-size: 30px;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      animation: floatHearts 10s linear infinite;
    }

    @keyframes floatHearts {
      0% { transform: translate(-50%, -50%) scale(1); opacity: 1; }
      100% { transform: translate(-50%, -200%) scale(2); opacity: 0; }
    }

    .scroll-msg {
      font-size: 16px;
      color: #ff1493;
      margin-top: 10px;
      animation: blink 1s step-start infinite;
      z-index: 10;
      position: relative;
    }

    @keyframes blink {
      50% { opacity: 0; }
    }

    /* Responsive */
    @media (max-width: 600px) {
      .cake { font-size: 36px; }
      .name { font-size: 24px; }
      .click-box { font-size: 20px; padding: 16px 32px; }
      .message {
        font-size: 20px;
        padding: 20px;
        max-width: 95%;
      }
      .heart-box {
        font-size: 80px;
      }
      .slideshow-section img {
        width: 95vw;
        max-width: 100%;
      }
      .zoom-label {
        font-size: 28px;
        top: 110px;
        left: 20px;
      }
      .arrow {
        font-size: 34px;
      }
    }
  </style>
</head>
<body>
  <!-- Romantic hearts blooming canvas -->
  <canvas id="loveCanvas"></canvas>

  <div class="stars"></div>
  <div class="hearts"></div>

  <div class="music-disc"></div>
  <div class="zoom-label">Zoom Out <span class="arrow">➠</span></div>

  <div class="container">
    <div class="click-box" onclick="startSurprise()">Click Me 💝</div>

    <div class="cake-section" id="cake">
      <div class="cake">🎂 Happy 19th Birthday 🎂</div>
      <div class="name">Tuuaa Raniii ❤️❤️😘</div>
      <div class="scroll-msg">⬇️ Scroll down to reveal your surprise... ⬇️</div>
    </div>

    <div class="message-section" id="wish">
      <div class="message">
        Happy 19th Birthday my love! ❤️ You make my world brighter every day. Your smile, your kindness, and your heart mean everything to me. I'm so lucky to have you in my life. May this year bring you endless happiness, laughter, and love. I love you more than words can say, Tuuaa Raniii! 😘💕
      </div>
    </div>

    <div class="gift-section" id="gift">
      <div class="heart-box" onclick="openGift()">❤️</div>
      <div class="message">Click the heart to open your surprise!</div>
    </div>

    <div class="slideshow-section" id="slideshow">
      <img src="img1.jpg" />
      <img src="img2.jpg" />
      <img src="img4.jpg" />
      <img src="img5.jpg" />
      <img src="img6.jpg" />
      <img src="img7.jpg" />
      <img src="img9.jpg" />
      <img src="img10.jpg" />
    </div>
  </div>

  <audio id="romanticAudio">
    <source src="romantic.mp3" type="audio/mpeg" />
  </audio>

  <script>
    // Canvas love hearts animation
    const canvas = document.getElementById('loveCanvas');
    const ctx = canvas.getContext('2d');
    let width, height;
    let hearts = [];

    const loveSymbols = ['❤️', '💖', '💕', '💘', '💞', '💓', '😘', '❣️'];

    function random(min, max) {
      return Math.random() * (max - min) + min;
    }

    function Heart() {
      this.x = random(0, width);
      this.y = random(height, height + 100);
      this.size = random(14, 30);
      this.speed = random(0.5, 1.5);
      this.opacity = 0;
      this.opacitySpeed = 0.01 + Math.random() * 0.02;
      this.symbol = loveSymbols[Math.floor(random(0, loveSymbols.length))];
      this.bloomScale = 1;
      this.bloomDirection = 1; // 1 growing, -1 shrinking
    }

    Heart.prototype.update = function() {
      this.y -= this.speed;
      if(this.opacity < 1) {
        this.opacity += this.opacitySpeed;
      }
      // Blooming effect
      this.bloomScale += this.bloomDirection * 0.005;
      if(this.bloomScale >= 1.15) this.bloomDirection = -1;
      else if(this.bloomScale <= 1) this.bloomDirection = 1;

      if(this.y < -50) {
        this.x = random(0, width);
        this.y = height + random(20, 100);
        this.size = random(14, 30);
        this.speed = random(0.5, 1.5);
        this.opacity = 0;
        this.symbol = loveSymbols[Math.floor(random(0, loveSymbols.length))];
      }
    }

    Heart.prototype.draw = function() {
      ctx.save();
      ctx.globalAlpha = this.opacity;
      ctx.font = `${this.size * this.bloomScale}px 'Segoe UI Emoji', 'Segoe UI', sans-serif`;
      ctx.fillStyle = `rgba(255, 20, 147, ${this.opacity})`;
      ctx.textAlign = 'center';
      ctx.shadowColor = `rgba(255, 105, 180, ${this.opacity})`;
      ctx.shadowBlur = 8;
      ctx.fillText(this.symbol, this.x, this.y);
      ctx.restore();
    }

    function init() {
      resize();
      hearts = [];
      for(let i=0; i < 40; i++) {
        hearts.push(new Heart());
      }
      animate();
    }

    function resize() {
      width = window.innerWidth;
      height = window.innerHeight;
      canvas.width = width;
      canvas.height = height;
    }

    function animate() {
      ctx.clearRect(0, 0, width, height);
      hearts.forEach(h => {
        h.update();
        h.draw();
      });
      requestAnimationFrame(animate);
    }

    window.addEventListener('resize', resize);
    init();

    // Your existing functions
    function startSurprise() {
      document.querySelector('.click-box').style.display = 'none';
      const audio = document.getElementById('romanticAudio');
      audio.play().catch(e => {
        console.log("User interaction needed to play audio.");
      });
      document.getElementById('cake').style.display = 'flex';
      setTimeout(() => {
        document.getElementById('wish').style.display = 'flex';
      }, 2000);
      setTimeout(() => {
        document.getElementById('gift').style.display = 'flex';
      }, 4000);
    }

    function openGift() {
      document.querySelector('.heart-box').style.display = 'none';
      const giftMessage = document.querySelector('#gift .message');
      giftMessage.textContent = "Here's your surprise! 🎉 Enjoy the music and photos!";
      explodeFireworks();
      setTimeout(() => {
        document.getElementById('gift').style.display = 'none';
        startSlideshow();
      }, 2500);
    }

    function explodeFireworks() {
      for (let i = 0; i < 40; i++) {
        const fw = document.createElement('div');
        fw.classList.add('firework');
        fw.style.left = Math.random() * window.innerWidth + 'px';
        fw.style.top = Math.random() * window.innerHeight + 'px';
        document.body.appendChild(fw);
        setTimeout(() => fw.remove(), 1200);
      }
    }

    function startSlideshow() {
      const slideshow = document.getElementById('slideshow');
      const images = slideshow.querySelectorAll('img');
      slideshow.style.display = 'flex';
      let i = 0;
      function showNext() {
        images.forEach(img => img.style.display = 'none');
        images[i].style.display = 'block';
        i = (i + 1) % images.length;
        setTimeout(showNext, 2500);
      }
      showNext();
    }
  </script>
</body>
</html>
