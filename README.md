<!DOCTYPE html>
<html>
<head>
  <title>Valentine 💘</title>
  <style>
    body {
      background-color: #ffe6e6;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: Arial, sans-serif;
    }

    #valentineBox {
      background-color: #fff0f5;
      border: 2px solid #cc0000;
      border-radius: 20px;
      padding: 30px;
      text-align: center;
      width: 350px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      position: relative;
    }

    h1 {
      color: #cc0000;
      margin-bottom: 10px;
    }

    p {
      font-size: 18px;
      margin-bottom: 20px;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 10px;
      border: none;
      cursor: pointer;
      margin: 5px;
      transition: all 0.2s;
      position: relative;
    }

    #yesBtn {
      background-color: #ff4d4d;
      color: white;
    }

    #noBtn {
      background-color: #cccccc;
    }

    img {
      width: 100px;
      margin-bottom: 15px;
      border-radius: 15px;
    }
  </style>
</head>
<body>
  <div id="valentineBox">
    <h1>💖 Sophie 💖</h1>
    <img src="https://cataas.com/cat/cute?size=100x100" alt="Cute cat with flowers">
    <p>Would you be my Valentine?</p>
    <button id="yesBtn">YES</button>
    <button id="noBtn">NO</button>
  </div>

  <script>
    const noBtn = document.getElementById('noBtn');

    noBtn.addEventListener('mouseenter', () => {
      const maxX = 220; // max horizontal movement
      const maxY = 80;  // max vertical movement
      const x = Math.random() * maxX;
      const y = Math.random() * maxY;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    });

    const yesBtn = document.getElementById('yesBtn');
    yesBtn.addEventListener('click', () => {
      alert("Yay! 💖 Sophie said YES!");
    });
  </script>
</body>
</html>


