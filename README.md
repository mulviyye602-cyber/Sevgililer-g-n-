# Sevgililer-g-n-
Seni cok seviyorum
<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sevgililer Günün Kutlu Olsun!</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      text-align: center;
      background: linear-gradient(to right, #ffafbd, #ffc3a0);
      margin: 0;
      padding: 0;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
    h1 {
      color: #fff;
      font-size: 3em;
      margin-bottom: 20px;
      text-shadow: 2px 2px 5px #ff5e62;
    }
    p {
      color: #fff;
      font-size: 1.5em;
      max-width: 500px;
      margin: 10px;
      text-shadow: 1px 1px 3px #ff5e62;
    }
    button {
      padding: 15px 30px;
      font-size: 1.2em;
      border: none;
      border-radius: 10px;
      background-color: #ff5e62;
      color: #fff;
      cursor: pointer;
      margin-top: 20px;
      transition: all 0.3s;
    }
    button:hover {
      background-color: #ff3b3f;
      transform: scale(1.1);
    }
    .hearts {
      position: absolute;
      width: 20px;
      height: 20px;
      background-color: red;
      transform: rotate(-45deg);
      animation: fly 2s linear forwards;
    }
    .hearts::after, .hearts::before {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background-color: red;
      border-radius: 50%;
    }
    .hearts::before {
      top: -10px;
      left: 0;
    }
    .hearts::after {
      left: 10px;
      top: 0;
    }
    @keyframes fly {
      0% {opacity: 1; transform: translateY(0) rotate(-45deg);}
      100% {opacity: 0; transform: translateY(-500px) rotate(-45deg);}
    }
  </style>
</head>
<body>
  <h1>Sevgililer Günün Kutlu Olsun! 💖</h1>
  <p>Canım, sen hayatımın en güzel hediyesisin. Her anım seninle daha da güzel!</p>
  <button onclick="sendLove()">Seni Seviyorum ❤️</button>

  <script>
    function sendLove() {
      for(let i = 0; i < 30; i++){
        let heart = document.createElement('div');
        heart.className = 'hearts';
        heart.style.left = Math.random() * window.innerWidth + 'px';
        heart.style.animationDuration = (Math.random() * 2 + 2) + 's';
        document.body.appendChild(heart);
        setTimeout(() => {
          heart.remove();
        }, 4000);
      }
      alert("❤️❤️❤️ Seni Seviyorum! ❤️❤️❤️");
    }
  </script>
</body>
</html>
