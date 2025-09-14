
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Google</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      background: #fff;
    }
    .logo {
      font-size: 64px;
      font-weight: bold;
      color: #4285F4;
      font-family: Arial, sans-serif;
      margin-bottom: 30px;
    }
    .logo span:nth-child(2) { color: #EA4335; }
    .logo span:nth-child(3) { color: #FBBC05; }
    .logo span:nth-child(4) { color: #4285F4; }
    .logo span:nth-child(5) { color: #34A853; }
    .logo span:nth-child(6) { color: #EA4335; }
    .search-box {
      display: flex;
      align-items: center;
      border: 1px solid #dcdcdc;
      border-radius: 24px;
      padding: 10px 20px;
      width: 400px;
      max-width: 80%;
    }
    .search-box input {
      flex: 1;
      border: none;
      outline: none;
      font-size: 16px;
    }
    .btn {
      margin-top: 20px;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      background-color: #f8f9fa;
      cursor: pointer;
      font-size: 14px;
    }
    .result {
      margin-top: 40px;
      font-size: 24px;
      font-weight: bold;
      color: #333;
    }
  </style>
</head>
<body>
  <div class="logo">
    <span>G</span><span>o</span><span>o</span><span>g</span><span>l</span><span>e</span>
  </div>
  <div class="search-box">
    <input type="text" id="searchInput" placeholder="Search Google">
  </div>
  <button class="btn" onclick="search()">Google Search</button>

  <div class="result" id="result"></div>

  <script>
    function search() {
      const query = document.getElementById("searchInput").value.trim().toLowerCase();
      const resultDiv = document.getElementById("result");
      if (query === "good boy") {
        resultDiv.textContent = "searching for CHARAN";
      } else {
        resultDiv.textContent = "Network Error";
      }
    }
  </script>
</body>
</html>
