<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cute Bear Valentine</title>
<style>
  body {
    background: linear-gradient(135deg, #ffe6f2, #ffb6c1);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    font-family: "Poppins", sans-serif;
    overflow: hidden;
  }

  .container {
    text-align: center;
    background: rgba(255, 255, 255, 0.7);
    padding: 20px 30px;
    border-radius: 20px;
    box-shadow: 0 4px 20px rgba(255, 0, 0, 0.2);
  }

  h2 {
    color: #ff4081;
    font-size: 22px;
    margin-top: 15px;
  }

  .buttons {
    margin-top: 20px;
    position: relative;
    height: 60px;
  }

  button {
    font-size: 18px;
    padding: 10px 25px;
    border: none;
    border-radius: 15px;
    cursor: pointer;
    transition: 0.3s;
    position: absolute;
  }

  #yes {
    left: 30%;
    background: #ff4d6d;
    color: white;
    box-shadow: 0 0 15px rgba(255, 0, 0, 0.4);
  }

  #no {
    right: 30%;
    background: #ff809f;
    color: white;
  }

  .message {
    display: none;
    font-size: 20px;
    color: white;
    font-weight: bold;
    background: #ff6fa5;
    padding: 25px;
    border-radius: 25px;
    margin-top: 25px;
    box-shadow: 0 0 30px pink;
    animation: pop 1s ease-in-out;
  }

  @keyframes pop {
    0% { transform: scale(0); opacity: 0; }
    100% { transform: scale(1); opacity: 1; }
  }
</style>
</head>
<body>

<div class="container" id="main">
  <!-- 🩷 Cute flower bear GIF -->
  <div class="tenor-gif-embed" data-postid="25985373" data-share-method="host" data-aspect-ratio="1" data-width="100%">
    <a href="https://tenor.com/view/%E0%B8%94%E0%B8%AD%E0%B8%81%E0%B9%84%E0%B8%A1%E0%B9%89-flowers-gif-25985373">ดอกไม้ Flowers GIF</a>
    from <a href="https://tenor.com/search/%E0%B8%94%E0%B8%AD%E0%B8%81%E0%B9%84%E0%B8%A1%E0%B9%89-gifs">ดอกไม้ GIFs</a>
  </div>
  <h2>Can you be with me? 💍</h2>
  <div class="buttons">
    <button id="yes">Yes 💕</button>
    <button id="no">No 😢</button>
  </div>
</div>

<!-- 💖 Message + second GIF -->
<div class="message" id="loveMessage">
  <div>Don’t worry about anything,<br>I just want to love you 💖</div>
  <br>
  <div class="tenor-gif-embed" data-postid="635661530100699849" data-share-method="host" data-aspect-ratio="1" data-width="100%">
    <a href="https://tenor.com/view/bubu-dudu-sseeyall-gif-635661530100699849">Bubu Dudu Sseeyall Sticker</a>
    from <a href="https://tenor.com/search/bubu+dudu-stickers">Bubu Dudu Stickers</a>
  </div>
</div>

<script type="text/javascript" async src="https://tenor.com/embed.js"></script>

<script>
  const noBtn = document.getElementById('no');
  const yesBtn = document.getElementById('yes');
  const msg = document.getElementById('loveMessage');
  const main = document.getElementById('main');

  // 🩷 "Yes" click → show love message + 2nd GIF
  yesBtn.addEventListener('click', () => {
    main.style.display = 'none';
    document.body.style.background = 'url("https://i.pinimg.com/originals/9a/5b/ed/9a5bed2a3e4b8a68b5cc64dd4093b96a.gif") center/cover';
    msg.style.display = 'block';
  });

  // 😆 "No" hover → moves a little around near Yes
  noBtn.addEventListener('mouseover', () => {
    const moveX = (Math.random() - 0.5) * 200;
    const moveY = (Math.random() - 0.5) * 150;
    noBtn.style.transform = `translate(${moveX}px, ${moveY}px)`;
  });
</script>

</body>
</html>
