<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover" />
  <title>Happy Birthday Tuuaa Raniii ❤️❤️😘</title>

  <!-- ✅ Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

  <style>
    html, body {
      margin: 0;
      padding: 0;
      max-width: 100%;
      overflow-x: hidden;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #ffd6e8, #fff0f5);
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
    }

    .click-box:hover {
      background-color: #ff1493;
    }

    .cake-section, .message-section, .gift-section, .gallery-section, .slideshow-section {
      display: none;
      flex-direction: column;
      align-items: center;
      animation: fadeIn 2s ease forwards;
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
    }

    .message {
      max-width: 800px;
      font-size: 26px;
      line-height: 1.6;
      background: white;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(255, 105, 180, 0.3);
      width: 100%;
    }

    .heart-box {
      font-size: 100px;
      cursor: pointer;
      animation: pulse 1.5s infinite;
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
    }

    .heart {
      position: absolute;
      top: -20px;
      animation-name: fall;
      animation-timing-function: linear;
      color: #ff69b4;
    }

    @keyframes fall {
      0% {
        transform: translateY(0);
        opacity: 1;
      }
      100% {
        transform: translateY(100vh);
        opacity: 0.3;
      }
    }

    /* ✅ Improved Mobile Responsiveness */
    @media (max-width: 600px) {
      .cake {
        font-size: 30px;
        text-align: center;
      }

      .name {
        font-size: 22px;
        margin-bottom: 15px;
      }

      .click-box {
        font-size: 18px;
        padding: 14px 24px;
        width: 100%;
        max-width: 320px;
        margin: 80px auto 0;
      }

      .message {
        font-size: 18px;
        padding: 16px;
        line-height: 1.5;
        box-shadow: none;
        width: 95%;
      }

      .heart-box {
        font-size: 70px;
      }

      .scroll-msg {
        font-size: 14px;
      }

      .slideshow-section img {
        width: 95vw;
        max-width: 100%;
        height: auto;
      }

      .music-disc {
        width: 50px;
        height: 50px;
        bottom: 15px;
        right: 15px;
      }

      .firework {
        box-shadow: 0 0 10px #fff5fa, 0 0 15px #ff69b4;
      }

      .container {
        padding: 20px 10px;
      }

      .love-shower .heart {
        font-size: 12px !important;
      }
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

  <!-- 🎵 Music Disc -->
  <div class="music-disc"></div>

  <!-- ❤️ Love Shower Container -->
  <div class="love-shower" id="loveShower"></div>

  <!-- 🎶 Background Music -->
  <audio id="romanticAudio">
    <source src="romantic.mp3" type="audio/mpeg" />
  </audio>

  <script>
    function startSurprise() {
      document.querySelector('.click-box').style.display = 'none';
      const audio = document.getElementById('romanticAudio');
      audio.play().catch(e => console.log("User interaction needed to play audio."));
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

      // ❤️ Start love shower
      document.getElementById('loveShower').style.display = 'block';
      generateLoveShower();

      function showNext() {
        images.forEach(img => img.style.display = 'none');
        images[i].style.display = 'block';
        i = (i + 1) % images.length;
        setTimeout(showNext, 2500);
      }
      showNext();
    }

    // ❤️ Love Shower Generator
    function generateLoveShower() {
      setInterval(() => {
        const heart = document.createElement('div');
        heart.className = 'heart';
        heart.textContent = '💖';
        heart.style.left = Math.random() * 100 + 'vw';
        heart.style.fontSize = (10 + Math.random() * 20) + 'px';
        heart.style.animationDuration = (3 + Math.random() * 3) + 's';
        document.getElementById('loveShower').appendChild(heart);
        setTimeout(() => heart.remove(), 7000);
      }, 100);
    }
  </script>
</body>
</html>

