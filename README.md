<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Merry Christmas & Happy New Year</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(120deg, #0f2027, #203a43, #2c5364);
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      overflow: hidden;
      text-align: center;
    }

    .card {
      background: rgba(255, 255, 255, 0.1);
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 0 30px rgba(255,255,255,0.2);
      animation: fadeIn 2s ease;
      max-width: 500px;
    }

    h1 {
      font-size: 42px;
      margin-bottom: 10px;
    }

    h2 {
      font-size: 32px;
      color: #ffeb3b;
      margin-bottom: 20px;
    }

    p {
      font-size: 18px;
      line-height: 1.6;
    }

    .footer {
      margin-top: 25px;
      font-style: italic;
      opacity: 0.8;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: scale(0.9);
      }
      to {
        opacity: 1;
        transform: scale(1);
      }
    }

    /* Snow animation */
    .snow {
      position: absolute;
      top: -10px;
      color: white;
      font-size: 12px;
      animation: fall linear infinite;
      opacity: 0.8;
    }

    @keyframes fall {
      to {
        transform: translateY(110vh);
      }
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>🎄 Merry Christmas 🎄</h1>
    <h2>& Happy New Year 🎆</h2>
    <p>
      Semoga damai Natal memenuhi hatimu,<br>
      dan Tahun Baru membawa harapan baru,<br>
      kebahagiaan, kesehatan, serta kesuksesan<br>
      di setiap langkahmu. Happy New year Rin!!! thanks for come to my lifeee ❤️❤️❤️
    </p>
    <p>
      Terima kasih untuk semua cerita di tahun ini.<br>
      Mari sambut tahun yang baru dengan senyum dan semangat baru ✨
    </p>
    <div class="footer">
      — With Love ❤️
    </div>
  </div>

  <script>
    function createSnow() {
      const snow = document.createElement("div");
      snow.className = "snow";
      snow.innerHTML = "❄";
      snow.style.left = Math.random() * window.innerWidth + "px";
      snow.style.animationDuration = (Math.random() * 3 + 2) + "s";
      document.body.appendChild(snow);

      setTimeout(() => {
        snow.remove();
      }, 5000);
    }

    setInterval(createSnow, 200);
  </script>

</body>
</html>
