
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday Tuuaa Raniii ❤️❤️😘</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #ffd6e8, #fff0f5);
      overflow-x: hidden;
      position: relative;
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
    }

    .click-box:hover {
      background-color: #ff1493;
    }

    .cake-section, .message-section, .gift-section, .slideshow-section {
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

    /* ✅ Music Disc - Bottom Right */
    .music-disc {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 80px;
      height: 80px;
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
    }

    @keyframes blink {
      50% { opacity: 0; }
    }

    /* ✅ Love Shower */
    .love-shower {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      overflow: hidden;
      pointer-events: none;
      z-index: 1;
    }

    .heart {
      position: absolute;
      color: #ff69b4;
      opacity: 0.8;
      font-size: 14px;
      animation: fall infinite linear;
      user-select: none;
      will-change: transform;
      filter: drop-shadow(0 0 2px #ff1493);
    }

    @keyframes fall {
      0% {
        transform: translateY(-10vh) scale(1);
        opacity: 1;
      }
      100% {
        transform: translateY(110vh) scale(1.2);
        opacity: 0;
      }
    }

    /* ✅ Responsive */
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
    }
  </style>
</head>

<body>
  <div class="stars"></div>
  <div class="hearts"></div>

  <div class="music-disc"></div>

  <div class="container">
    <div class="click-box" onclick="startSurprise()">Click Me 💝</div>

    <div class="cake-section" id="cake">
      <div class="cake">🎂 Happy 19th Birthday 🎂</div>
      <div class="name">Tuuaa Raniii ❤️❤️😘</div>
      <div class="scroll-msg">⬇️ Scroll down to reveal your surprise... ⬇️</div>
    </div>

    <div class="message-section" id="wish">
      <div class="message">
        Happy 19th Birthday my love! ❤️ You make my world brighter every day.
        Your smile, your kindness, and your heart mean everything to me.
        I'm so lucky to have you in my life. May this year bring you endless
        happiness, laughter, and love. I love you more than words can say,
        Tuuaa Raniii! 😘💕
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

  <!-- ❤️ Love Shower Container -->
  <div class="love-shower" id="loveShower"></div>

  <audio id="romanticAudio">
    <source src="romantic.mp3" type="audio/mpeg" />
  </audio>

  <script>
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
        startLoveShower();
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

    // ❤️ Love Shower Function
    function startLoveShower() {
      const container = document.getElementById('loveShower');
      container.style.display = 'block';

      const numberOfHearts = 80;

      for (let i = 0; i < numberOfHearts; i++) {
        const heart = document.createElement('div');
        heart.className = 'heart';
        heart.innerText = '❤️';

        const size = Math.random() * 12 + 8; // 8px to 20px
        heart.style.fontSize = `${size}px`;

        heart.style.left = `${Math.random() * 100}vw`;

        const duration = Math.random() * 3 + 4; // 4s to 7s
        const delay = Math.random() * 5; // random delay

        heart.style.animationDuration = `${duration}s`;
        heart.style.animationDelay = `${delay}s`;

        container.appendChild(heart);

        // Reset when animation loops
        heart.addEventListener('animationiteration', () => {
          heart.style.left = `${Math.random() * 100}vw`;
          heart.style.animationDuration = `${Math.random() * 3 + 4}s`;
        });
      }
    }
  </script>
</body>
</html>

