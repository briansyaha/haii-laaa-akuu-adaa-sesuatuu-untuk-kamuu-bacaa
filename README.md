# haaii-laa-akuu-adaa-sesuatuu untuk kamu bacaaa
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Untuk muuu laaa</title>
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Open+Sans&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Open Sans', sans-serif;
      background: linear-gradient(to bottom right, #ffc1cc, #ffe4ec);
      color: #333;
      text-align: center;
      overflow-x: hidden;
    }
    h1 {
      font-family: 'Pacifico', cursive;
      font-size: 2.5em;
      color: #d63384;
      margin-top: 20px;
    }
    .message {
      max-width: 90%;
      margin: 20px auto;
      background: white;
      padding: 20px;
      border-radius: 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    img {
      max-width: 80%;
      margin: 10px auto;
      border-radius: 20px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }
    .animation {
      position: fixed;
      width: 100%;
      height: 100%;
      pointer-events: none;
      overflow: hidden;
      z-index: 0;
    }
    .heart, .flower {
      position: absolute;
      font-size: 24px;
      animation: float 6s infinite;
      opacity: 0.7;
    }
    @keyframes float {
      0% { transform: translateY(100vh) rotate(0deg); opacity: 0; }
      50% { opacity: 0.8; }
      100% { transform: translateY(-10vh) rotate(360deg); opacity: 0; }
    }
    audio {
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="animation" id="animation"></div>

  <h1>Untukkk muuu laaaa</h1>
  <div class="message">
    <p>Jika kamu sedang merasa tidak baik-baik saja, ingatlah selalu laaaa ada aku untukmu berbagi cerita apa pun ituuu.<br>
    Selamat National Girlfriend Day laaaaa 💐.maaf yaaa akuu baruu cumaaa bisaa ngucapinnn😁(ian) </p>
  </div>

  <img src="IMG-20250719-WA0012.jpg" alt="foto1">
  <img src="IMG-20250719-WA0010.jpg" alt="foto2">

  <audio controls autoplay loop>
    <source src="https://youtu.be/2Vv-BfVoq4g?si=nB72kpqnxIO9WB9U" type="audio/mp3">

  <script>
    const animationContainer = document.getElementById('animation');
    const emojis = ['❤️', '🌸', '💕', '🌹'];
    function createEmoji() {
      const emoji = document.createElement('div');
      emoji.classList.add('heart');
      emoji.style.left = Math.random() * 100 + 'vw';
      emoji.style.top = '100vh';
      emoji.textContent = emojis[Math.floor(Math.random() * emojis.length)];
      emoji.style.fontSize = (20 + Math.random() * 20) + 'px';
      emoji.style.animationDuration = (4 + Math.random() * 3) + 's';
      animationContainer.appendChild(emoji);

      setTimeout(() => {
        emoji.remove();
      }, 7000);
    }

    setInterval(createEmoji, 500);
  </script>
</body>
</html>
