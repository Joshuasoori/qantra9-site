<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>QANTRA-9</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden;
      font-family: 'Orbitron', sans-serif;
      background: black;
      color: white;
    }

    body::before {
      content: "";
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      background: url("space-bg.png") center/cover no-repeat;
      animation: flicker 5s infinite;
      z-index: -2;
    }

    @keyframes flicker {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.85; }
    }

    .tree {
      position: absolute;
      top: 20%;
      left: 50%;
      transform: translateX(-50%);
      width: 200px;
      height: 200px;
      background: radial-gradient(circle, #00f0ff 0%, transparent 70%);
      border-radius: 50%;
      filter: blur(30px);
      animation: glow 4s ease-in-out infinite;
    }

    @keyframes glow {
      0%, 100% { opacity: 0.6; }
      50% { opacity: 1; }
    }

    .content {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
    }

    h1 {
      font-size: 2.5rem;
      text-shadow: 0 0 10px #0ff, 0 0 30px #00f;
    }

    p {
      color: #0ff;
      font-size: 1.2rem;
      text-shadow: 0 0 10px #0ff;
    }

    audio {
      display: none;
    }
  </style>
</head>
<body>

  <div class="tree"></div>

  <div class="content">
    <h1>THE SIGNAL IS NOT COMING...<br><span style="color:#00f0ff;">QANTRA-9</span><br>IT HAS ALREADY BEGUN.</h1>
    <p>— "Not from Earth"</p>
    <audio autoplay loop>
      <source src="https://files.catbox.moe/tp5mb2.mp3" type="audio/mpeg">
    </audio>
  </div>

</body>
</html>
