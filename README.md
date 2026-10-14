# 2026_ds

<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hello World</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding-top: 100px;
      background: #f5f5f5;
    }

    button {
      padding: 12px 24px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      background: #333;
      color: white;
      cursor: pointer;
    }

    button:hover {
      background: #555;
    }

    #message {
      margin-top: 30px;
      font-size: 42px;
      font-weight: bold;
    }

    .rainbow {
      background: linear-gradient(
        90deg,
        red,
        orange,
        yellow,
        green,
        blue,
        indigo,
        violet
      );
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      background-size: 200% auto;
      animation: rainbow 3s linear infinite;
    }

    @keyframes rainbow {
      to {
        background-position: 200% center;
      }
    }
  </style>
</head>

<body>

  <h1>Hello World</h1>

  <button id="helloButton">
    クリックしてください
  </button>

  <div id="message"></div>

  <script>
    const button = document.getElementById("helloButton");
    const message = document.getElementById("message");

    button.addEventListener("click", function () {
      message.textContent = "Hello world";
      message.classList.add("rainbow");
    });
  </script>

</body>
</html>
