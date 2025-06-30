<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<style>
  @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap');

  body {
    background: #fff;
    text-align: center;
    font-family: Arial, sans-serif;
  }
  .heart {
    width: 100px;
    height: 100px;
    background: red;
    position: relative;
    transform: rotate(-45deg);
    animation: pulse 1s infinite;
    margin: 100px auto;
  }
  .heart::before,
  .heart::after {
    content: '';
    width: 100px;
    height: 100px;
    background: red;
    border-radius: 50%;
    position: absolute;
  }
  .heart::before {
    top: -50px;
    left: 0;
  }
  .heart::after {
    left: 50px;
    top: 0;
  }

  @keyframes pulse {
    0% { transform: rotate(-45deg) scale(1); }
    50% { transform: rotate(-45deg) scale(1.2); }
    100% { transform: rotate(-45deg) scale(1); }
  }

  .text {
    font-size: 26px;
    color: #d10000;
    margin-top: 20px;
    font-family: 'Great Vibes', cursive;
    animation: fade 2s infinite alternate;
    font-weight: bold;
  }

  @keyframes fade {
    0% { opacity: 0.3; }
    100% { opacity: 1; }
  }
</style>
</head>
<body>
<div class="heart"></div>
<div class="text">======Nayani Manikah======</div>
</body>
</html>
