<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Birthday Surprise</title>
<style>
    html, body {
        margin: 0;
        padding: 0;
        height: auto;
        min-height: 100vh;
        overflow-x: hidden;
        overflow-y: auto;
        font-family: 'Arial', sans-serif;
        background: #ffeef3;
    }

    .center {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100vh;
        flex-direction: column;
        text-align: center;
    }

    .hidden { display: none; }

    .click-box {
        cursor: pointer;
        background: #ff4f81;
        padding: 20px 40px;
        border-radius: 12px;
        color: #fff;
        font-size: 1.5em;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        transition: background 0.3s;
    }

    .click-box:hover {
        background: #ff2365;
    }

    #cake, #wish, #gift {
        display: none;
        flex-direction: column;
        align-items: center;
        padding: 20px;
    }

    #loveTree {
        position: relative;
        width: 300px;
        height: 400px;
        margin: 20px auto;
    }

    .heart {
        position: absolute;
        color: #ff4f81;
        font-size: 20px;
        animation: float 6s infinite ease-in-out;
    }

    @keyframes float {
        0% { transform: translateY(0) scale(1); opacity: 1; }
        50% { transform: translateY(-30px) scale(1.2); opacity: 0.7; }
        100% { transform: translateY(0) scale(1); opacity: 1; }
    }

    .note {
        background: rgba(255,255,255,0.9);
        padding: 15px;
        border-radius: 10px;
        text-align: center;
        font-size: 1.2em;
        color: #333;
        max-width: 250px;
        margin: auto;
        box-shadow: 0 3px 10px rgba(0,0,0,0.2);
    }

    img {
        max-width: 90%;
        height: auto;
        margin-top: 10px;
        border-radius: 10px;
        box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
</style>
</head>
<body>

<!-- Intro Screen -->
<div class="center" id="introScreen">
    <div class="click-box" onclick="startSurprise()">🎁 Tap to Open Gift</div>
</div>

<!-- Cake -->
<div class="center" id="cake">
    <h1>🎂 Happy Birthday! 🎂</h1>
    <img src="cake.jpg" alt="Birthday Cake">
</div>

<!-- Wish -->
<div class="center" id="wish">
    <div id="loveTree"></div>
    <div class="note">You are the sweetest part of my life ❤️</div>
</div>

<!-- Gift Photos -->
<div class="center" id="gift">
    <h2>Special Memories 🎉</h2>
    <img src="photo1.jpg" alt="Memory 1">
    <img src="photo2.jpg" alt="Memory 2">
</div>

<audio id="romanticAudio" src="romantic.mp3"></audio>

<script>
function startSurprise() {
    // Hide intro
    document.getElementById('introScreen').style.display = 'none';

    // Always show visuals
    document.getElementById('cake').style.display = 'flex';
    setTimeout(() => {
        document.getElementById('wish').style.display = 'flex';
        createLoveTree();
    }, 2000);
    setTimeout(() => {
        document.getElementById('gift').style.display = 'flex';
    }, 4000);

    // Try to play music (won't stop visuals if blocked)
    const audio = document.getElementById('romanticAudio');
    audio.play().catch(() => {
        console.log("Music autoplay blocked, continuing visuals.");
    });
}

function createLoveTree() {
    const tree = document.getElementById('loveTree');
    tree.innerHTML = '';
    for (let i = 0; i < 30; i++) {
        const heart = document.createElement('div');
        heart.className = 'heart';
        heart.textContent = '❤';
        heart.style.left = Math.random() * 280 + 'px';
        heart.style.top = Math.random() * 380 + 'px';
        heart.style.animationDelay = (Math.random() * 5) + 's';
        tree.appendChild(heart);
    }
}
</script>

</body>
</html>

