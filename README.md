# AngelJane
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Valentine </title>
  <style>
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #ffd6e8, #ffeef5);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .card {
      background: white;
      padding: 30px 25px;
      border-radius: 20px;
      text-align: center;
      max-width: 320px;
      width: 90%;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    }

    h1 {
      font-size: 22px;
      color: #e75480;
      margin-bottom: 20px;
    }

    button {
      border: none;
      padding: 12px 20px;
      border-radius: 25px;
      font-size: 16px;
      cursor: pointer;
      margin: 10px;
    }

    #yes {
      background: #ff5c8a;
      color: white;
    }

    #no {
      background: #eee;
      color: #555;
      position: relative;
    }

    .message {
      font-size: 18px;
      color: #e75480;
      margin-top: 20px;
      display: none;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Angel Jane,<br>will you be my Valentine? 💖</h1>

    <button id="yes">Yes 💕</button>
    <button id="no">No 🙈</button>

    <div class="message" id="msg">
      Yunn Ohh Bagoo pa HAHAHAHA😆❤️
    </div>
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");
    const msg = document.getElementById("msg");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 200 - 100;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    });

    yesBtn.addEventListener("click", () => {
      msg.style.display = "block";
      yesBtn.style.display = "none";
      noBtn.style.display = "none";
    });
  </script>

</body>
</html>
