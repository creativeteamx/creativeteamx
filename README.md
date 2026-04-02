<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Creative Team - Lead Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #0a0a0a;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .container {
      text-align: center;
      background: #111;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 0 20px rgba(0, 200, 255, 0.3);
      width: 300px;
    }

    .logo {
      width: 200px;
      margin-bottom: 20px;
    }

    h2 {
      margin-bottom: 20px;
      color: #00c8ff;
    }

    input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 6px;
      border: none;
      outline: none;
    }

    button {
      width: 100%;
      padding: 10px;
      background: #00c8ff;
      color: black;
      border: none;
      border-radius: 6px;
      font-weight: bold;
      cursor: pointer;
    }

    button:hover {
      background: #00a0cc;
    }
  </style>
</head>
<body>

  <div class="container">
    <!-- Replace 'logo.png' with your uploaded logo file name -->
    <img src="logo.png" alt="Creative Team Logo" class="logo">

    <h2>Get Started</h2>

    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="tel" placeholder="Phone Number" required>
      <button type="submit">Submit</button>
    </form>
  </div>

</body>
</html>
