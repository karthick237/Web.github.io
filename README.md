<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ID Verification Demo</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .container {
      background: white;
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      width: 350px;
      text-align: center;
    }
    h2 {
      color: #333;
    }
    input {
      width: 90%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    button {
      padding: 10px 20px;
      background: #007bff;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
    .result {
      margin-top: 15px;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>ID Verification Demo</h2>
    <input type="text" id="idNumber" placeholder="Enter Aadhaar / Voter ID">
    <button onclick="verifyID()">Verify</button>
    <div class="result" id="result"></div>
  </div>

  <script>
    function verifyID() {
      const id = document.getElementById("idNumber").value.trim();
      const result = document.getElementById("result");

      // Dummy verification logic
      const validIDs = ["123456789012", "ABC1234567", "987654321098"];

      if (validIDs.includes(id)) {
        result.innerHTML = "✅ ID Verified Successfully!";
        result.style.color = "green";
      } else {
        result.innerHTML = "❌ Invalid ID Number!";
        result.style.color = "red";
      }
    }
  </script>
</body>
</html>
# Web.github.io
