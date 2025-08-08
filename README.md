
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover" />
  <title>Happy Birthday Tuuaa Raniii ❤️❤️😘</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

  <style>
    html, body {
      margin: 0;
      padding: 0;
      max-width: 100%;
      overflow-x: hidden;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #ffd6e8, #fff0f5);
      height: 100%;
    }

    * {
      box-sizing: border-box;
    }

    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 30px;
      min-height: 100vh;
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
      max-width: 90%;
      user-select: none;
    }

    .click-box:hover {
      background-color: #ff1493;
    }

    .cake-section, .message-section, .gift-section, .slideshow-section {
      display: none;
      flex-direction: column;
      align-items: center;
      animation: fadeIn 2s ease forwards;
      width: 100%;
      max-width: 800px;
      margin: 20px auto;
    }

    .cake {
      font-size: 50px;
      margin: 40px 0 10px;
    }

    .name {
      font-size: 30px;
      font-weight: bold;
      color: #ff1493;
      margin-bottom: 20px;
      font-family: 'Dancing Script', cursive;
    }

    .message {
      font-size: 26px;
      line-height: 1.6;
      background: white;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(255, 105, 180, 0.3);
      width: 100%;
      user-select: none;
    }

    .heart-box {
      font-size: 100px;
      cursor: pointer;
      animation: pulse 1.5s infinite;
      user-select: none;
      color: #ff0000;
      text-shadow: 0 0 15px #ff0000, 0 0 30px #ff4d4d;
      margin-bottom: 10px;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
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
      pointer-events: none;
      user-select: none;
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
      user-select: none;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .music-disc {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 70px;
      height: 70px;
      border-radius: 50%;
      background: url('img3.jpg') no-repeat center/cover;
      border: 3px solid #ff69b4;
      animation: spin 5s linear infinite;
      box-shadow: 0 0 20px rgba(255, 192, 203, 0.7);
      z-index: 10;
      user-select: none;
    }

    @keyframes spin {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }

    .scroll-msg {
      font-size: 16px;
      color: #ff1493;
      margin-top: 10px;
      animation: blink 1s step-start infinite;
      user-select: none;
    }

    @keyframes blink {
      50% { opacity: 0; }
    }

    /* ❤️ Love Shower */
    .love-shower {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      pointer-events: none;
      overflow: hidden;
      z-index: 5;
      display: none;
      user-select: none;
    }

    .heart {
      position: absolute;
      top: -20px;
      color: red;
      text-shadow: 0 0 10px #ff0000, 0 0 20px #ff4d4d, 0 0 30px #ff6666;
      animation-name: fall;
      animation-timing-function: linear;
      user-select: none;
    }

    @keyframes fall {
      0% {
        transform: translateY(0);
        opacity: 1;
      }
      100% {
        transform: translateY(100vh);
        opacity: 0.2;
      }
    }

    /* Responsive Fixes */
    @media (max-width: 600px) {
      .container {
        padding: 20px;
        align-items: center;
        justify-content: center;
      }

      .cake { font-size: 36px; }
      .name { font-size: 24px; }
      .click-box { font-size: 20px; padding: 16px 32px; }
      .message { font-size: 20px; padding: 20px; }
      .heart-box { font-size: 80px; }
      .slideshow-section img { width: 95vw; max-width: 100%; }
      .music-disc { width: 60px; height: 60px; }
    }
  </style>
</head>

<body>
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
      <img src="img1.jpg" alt="Birthday photo 1" />
      <img src="img2.jpg" alt="Birthday photo 2" />
      <img src="img4.jpg" alt="Birthday photo 4" />
      <img src="img5.jpg" alt="Birthday photo 5" />
      <img src="img6.jpg" alt="Birthday photo 6" />
      <img src="img7.jpg" alt="Birthday photo 7" />
      <img src="img9.jpg" alt="Birthday photo 9" />
      <img src="img10.jpg" alt="Birthday photo 10" />
    </div>
  </div>

  <!-- Music Disc -->
  <div class="music-disc" aria-label="Rotating music disc"></div>

  <!-- Love Shower Container -->
  <div class="love-shower" id="loveShower" aria-hidden="true"></div>

  <!-- Background Music -->
  <audio id="romanticAudio" preload="auto">
    <source src="romantic.mp3" type="audio/mpeg" />
  </audio>

  <script>
    function startSurprise() {
      document.querySelector('.click-box').style.display = 'none';
      const audio = document.getElementById('romanticAudio');
      audio.play().catch(() => console.log("User interaction needed to play audio."));
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

      // Show the first image immediately
      images.forEach(img => img.style.display = 'none');
      images[0].style.display = 'block';

      // Start love shower hearts
      document.getElementById('loveShower').style.display = 'block';
      generateLoveShower();

      function showNext() {
        images.forEach(img => img.style.display = 'none');
        images[i].style.display = 'block';
        i = (i + 1) % images.length;
        setTimeout(showNext, 2500);
      }
      setTimeout(showNext, 2500);
    }

    // Love Shower Generator with red glowing hearts, centered horizontally
    function generateLoveShower() {
      setInterval(() => {
        const heart = document.createElement('div');
        heart.className = 'heart';
        heart.textContent = '❤️';
        // Centered horizontally between 25vw to 75vw (middle half)
        heart.style.left = (25 + Math.random() * 50) + 'vw';
        heart.style.fontSize = (15 + Math.random() * 25) + 'px';
        heart.style.animationDuration = (3 + Math.random() * 3) + 's';
        heart.style.opacity = 1;
        document.getElementById('loveShower').appendChild(heart);
        setTimeout(() => heart.remove(), 7000);
      }, 120);
    }
  </script>
</body>
</html>

