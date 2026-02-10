# Kriti-cutie-
Valiant
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Kriti 💖</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ffd6e8, #ffeaf4);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Comic Sans MS', 'Poppins', cursive;
      overflow: hidden;
    }

    .card {
      background: #fff0f6;
      padding: 40px 50px;
      border-radius: 30px;
      box-shadow: 0 15px 40px rgba(255, 105, 180, 0.3);
      text-align: center;
      max-width: 400px;
      position: relative;
    }

    h1 {
      color: #ff4d8d;
      font-size: 2.5rem;
      margin-bottom: 10px;
    }

    p {
      color: #ff6fa5;
      font-size: 1.1rem;
      margin-bottom: 30px;
    }

    button {
      background: #ff8fb1;
      border: none;
      padding: 15px 30px;
      border-radius: 50px;
      font-size: 1rem;
      color: white;
      cursor: not-allowed;
      opacity: 0.7;
    }

    button:hover {
      animation: shake 0.4s;
    }

    @keyframes shake {
      0% { transform: translateX(0); }
      25% { transform: translateX(-5px); }
      50% { transform: translateX(5px); }
      75% { transform: translateX(-5px); }
      100% { transform: translateX(0); }
    }

    .heart {
      position: absolute;
      color: #ff5d9e;
      font-size: 20px;
      animation: float 6s linear infinite;
      opacity: 0.7;
    }

    @keyframes float {
      0% {
        transform: translateY(0) scale(1);
        opacity: 0.8;
      }
      100% {
        transform: translateY(-800px) scale(1.5);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Kriti 💕</h1>
    <p>
      Happy Valentine’s Day 💘<br>
      This page is just for you.
    </p>
    <button>
      Nope 😌 You can’t press this
    </button>
  </div>

  <!-- Floating hearts -->
  <script>
    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.innerHTML = "💗";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.bottom = "-20px";
      heart.style.animationDuration = (4 + Math.random() * 3) + "s";
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 7000);
    }

    setInterval(createHeart, 400);
  </script>

</body>
</html>
