
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover" />
  <title>Happy Birthday Tuuaa Raniii ❤️❤️😘</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet" />

  <style>
    /* Reset & base */
    html, body {
      margin: 0; padding: 0;
      width: 100vw;
      height: 100vh;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to bottom right, #ffd6e8, #fff0f5);
      overflow-x: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      user-select: none;
    }

    body {
      flex-direction: column;
      padding: 15px;
      box-sizing: border-box;
    }

    .container {
      width: 100%;
      max-width: 400px; /* Mobile friendly width */
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }

    .click-box {
      background-color: #ff69b4;
      color: white;
      font-size: 22px;
      padding: 18px 0;
      border-radius: 12px;
      cursor: pointer;
      width: 100%;
      max-width: 320px;
      margin: 100px auto 0;
      box-shadow: 0 5px 15px rgba(255, 105, 180, 0.4);
      transition: background-color 0.3s ease;
    }
    .click-box:hover {
      background-color: #ff1493;
    }

    .cake-section, .message-section, .gift-section, .slideshow-section {
      display: none;
      flex-direction: column;
      align-items: center;
      animation: fadeIn 1.5s ease forwards;
      margin-top: 30px;
      width: 100%;
    }

    .cake {
      font-size: 36px;
      margin: 20px 0 10px;
      user-select: none;
    }

    .name {
      font-family: 'Dancing Script', cursive;
      font-size: 26px;
      font-weight: 700;
      color: #ff1493;
      margin-bottom: 15px;
      user-select: none;
    }

    .scroll-msg {
      font-size: 14px;
      color: #ff1493;
      animation: blink 1.2s step-start infinite;
      margin-top: -10px;
      user-select: none;
    }

    .message {
      font-size: 20px;
      line-height: 1.5;
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 0 12px rgba(255, 105, 180, 0.3);
      width: 100%;
      user-select: none;
      word-break: break-word;
    }

    .heart-box {
      font-size: 80px;
      color: #ff0000;
      cursor: pointer;
      animation: pulse 1.5s infinite;
      margin-bottom: 12px;
      text-shadow: 0 0 15px #ff0000, 0 0 25px #ff4d4d;
      user-select: none;
    }

    /* Fireworks */
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
      z-index: 9999;
    }

    /* Slideshow */
    .slideshow-section {
      display: none;
      flex-direction: column;
      align-items: center;
      margin-top: 30px;
      width: 100%;
      max-width: 320px;
    }

    .slideshow-section img {
      width: 100%;
      border-radius: 15px;
      box-shadow: 0 0 20px rgba(255, 105, 180, 0.5);
      display: none;
      animation: fadeIn 1s ease forwards;
      user-select: none;
    }

    /* Music Disc */
    .music-disc {
      position: fixed;
      bottom: 15px;
      right: 15px;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      background: url('img3.jpg') no-repeat center/cover;
      border: 3px solid #ff69b4;
      animation: spin 5s linear infinite;
      box-shadow: 0 0 15px rgba(255, 192, 203, 0.7);
      z-index: 1000;
      user-select: none;
    }

    /* Love shower hearts container */
    .love-shower {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      pointer-events: none;
      overflow: hidden;
      z-index: 900;
      display: none;
      user-select: none;
    }

    .heart {
      position: absolute;
      top: -20px;
      color: #ff0000;
      text-shadow: 0 0 10px #ff0000, 0 0 20px #ff4d4d, 0 0 30px #ff6666;
      animation-name: fall;
      animation-timing-function: linear;
      user-select: none;
    }

    /* Animations */
    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(20px);}
      to {opacity: 1; transform: translateY(0);}
    }

    @keyframes blink {
      50% {opacity: 0;}
    }

    @keyframes pulse {
      0%, 100% {transform: scale(1);}
      50% {transform: scale(1.1);}
    }

    @keyframes explode {
      0% {transform: scale(1); opacity: 1;}
      100% {transform: scale(25); opacity: 0;}
    }

    @keyframes fall {
      0% {transform: translateY(0); opacity: 1;}
      100% {transform: translateY(100vh); opacity: 0.2;}
    }

    @keyframes spin {
      from {transform: rotate(0deg);}
      to {transform: rotate(360deg);}
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

  <div class="music-disc" aria-label="Rotating music disc"></div>

  <div class="love-shower" id="loveShower" aria-hidden="true"></div>

  <audio id="romanticAudio" preload="auto">
    <source src="romantic.mp3" type="audio/mpeg" />
  </audio>

  <script>
    function startSurprise() {
      const clickBox = document.querySelector('.click-box');
      clickBox.style.display = 'none';

      const audio = document.getElementById('romanticAudio');
      audio.play().catch(() => {
        console.log('User interaction required to play audio.');
      });

      document.getElementById('cake').style.display = 'flex';

      setTimeout(() => {
        document.getElementById('wish').style.display = 'flex';
      }, 1800);

      setTimeout(() => {
        document.getElementById('gift').style.display = 'flex';
      }, 3600);
    }

    function openGift() {
      const heartBox = document.querySelector('.heart-box');
      heartBox.style.display = 'none';

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
      images.forEach(img => (img.style.display = 'none'));
      images[0].style.display = 'block';

      document.getElementById('loveShower').style.display = 'block';
      generateLoveShower();

      function showNext() {
        images.forEach(img => (img.style.display = 'none'));
        images[i].style.display = 'block';
        i = (i + 1) % images.length;
        setTimeout(showNext, 2500);
      }
      setTimeout(showNext, 2500);
    }

    // Love Shower with red glowing hearts, centered horizontally
    function generateLoveShower() {
      setInterval(() => {
        const heart = document.createElement('div');
        heart.className = 'heart';
        heart.textContent = '❤️';
        // Center horizontally on screen between 25vw and 75vw
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


