<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Free Laptop for HS Survivors</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #ffe, #e0f7fa);
      color: #333;
      padding: 2em;
      text-align: center;
    }
    h1 { font-size: 2.5em; color: darkgreen; }
    h2 { font-size: 1.5em; color: #ff5722; }
    .container {
      max-width: 600px;
      margin: auto;
      background: white;
      padding: 2em;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }
    input, button {
      padding: 0.7em;
      margin: 1em;
      width: 80%;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      background-color: #4caf50;
      color: white;
      font-size: 1em;
      cursor: pointer;
    }
    .footer {
      margin-top: 2em;
      font-size: 0.8em;
      color: #777;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Congratulations, HS Warrior!</h1>
    <h2>You've Earned a Free Laptop!* (*Absolutely Maybe)</h2>
    <p>Because we *really* believe in students who just suffered through 3-hour exams and now trust shady websites.</p>
    
    <form onsubmit="showConfirmation(event)">
      <input type="file" accept=".pdf,.jpg,.jpeg,.png" required><br>
      <input type="text" placeholder="Enter Your HS Registration Number" required><br>
      <button type="submit">Upload & Claim 'Laptop'</button>
    </form>

    <div id="confirmation" style="display:none;">
      <h2>Your Upload is Under Sarcastic Review!</h2>
      <p>Our imaginary team is now processing your data in an intergalactic cloud server.</p>
      <p>If your laptop doesn't arrive in 10 minutes, please wait longer.</p>
    </div>

    <div class="footer">
      *Terms & conditions apply. Like, a lot. Also, there is no laptop. Just vibes.
    </div>
  </div>

  <script>
    function showConfirmation(event) {
      event.preventDefault();
      document.querySelector('form').style.display = 'none';
      document.getElementById('confirmation').style.display = 'block';
    }
  </script>
</body>
</html>
