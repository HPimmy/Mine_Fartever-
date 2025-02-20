<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Forever Yours</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Georgia', serif;
      background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 100%);
      color: #5a3e36;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      overflow: hidden;
      position: relative;
    }
    .container {
      background: rgba(255, 255, 255, 0.8);
      padding: 40px;
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
      max-width: 600px;
      animation: fadeIn 2s ease-in-out;
      position: relative;
      z-index: 2;
    }
    h1 {
      font-size: 3rem;
      margin-bottom: 20px;
      color: #5a3e36;
    }
    p {
      font-size: 1.5rem;
      line-height: 1.6;
      margin-bottom: 30px;
    }
    button {
      background: #ff6f61;
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 1.2rem;
      border-radius: 25px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button:hover {
      background: #ff3b2f;
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    /* Heart shower animation */
    .heart-shower {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none; /* Ensure clicks pass through */
      z-index: 3;
      display: none; /* Hidden by default */
    }

    .heart-shower span {
      position: absolute;
      display: block;
      width: 20px;
      height: 20px;
      background: url('https://i.imgur.com/9Q9Q9Q9.png') no-repeat center center/contain;
      animation: animateHearts 5s linear infinite;
      bottom: -150px;
    }

    @keyframes animateHearts {
      0% {
        transform: translateY(0) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(-1000px) rotate(720deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Will You Be Mine Forever?</h1>
    <p>
      My love, from the moment we met, you’ve brought so much joy and light into my life. 
      Every moment with you feels like a dream, and I never want to wake up. 
      You are my everything, and I can’t imagine doing life without you by my side.
    </p>
    <p>
      So would you wanna grow and giggle away in life with me???
      Let’s create a lifetime of beautiful memories together.
    </p>
    <button onclick="startHeartShower()">Yes, Forever!</button>
  </div>

  <!-- Heart shower -->
  <div class="heart-shower" id="heartShower">
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
  </div>

  <script>
    function startHeartShower() {
      // Show the heart shower
      const heartShower = document.getElementById('heartShower');
      heartShower.style.display = 'block';

      // Show an alert message
      alert('I knew you’d say yes! I love you endlessly. ❤️');
    }
  </script>
</body>
</html>
