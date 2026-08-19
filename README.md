<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Player UID</title>

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #111;
      color: white;
      text-align: center;
      padding-top: 80px;
    }

    .box {
      background: #222;
      padding: 25px;
      margin: 20px;
      border-radius: 15px;
    }

    input, button {
      padding: 12px;
      margin: 8px;
      border-radius: 8px;
      border: none;
      font-size: 16px;
    }

    button {
      cursor: pointer;
    }

    #result {
      margin-top: 20px;
      font-size: 20px;
    }
  </style>
</head>

<body>

  <div class="box">
    <h1>Free Fire Player</h1>

    <input type="text" id="uid" placeholder="Enter UID">

    <button onclick="showUID()">Show UID</button>

    <div id="result"></div>
  </div>

  <script>
    function showUID() {
      const uid = document.getElementById("uid").value;

      if (uid.trim() === "") {
        document.getElementById("result").innerText = "UID enter karo!";
        return;
      }

      document.getElementById("result").innerText =
        "Player UID: " + uid;
    }
  </script>

</body>
</html>
