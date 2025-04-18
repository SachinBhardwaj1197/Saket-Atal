<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saket Atal ki Rachnayen</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #222;
      transition: background-color 0.3s, color 0.3s;
    }

    header {
      background-color: #222;
      color: white;
      padding: 1rem;
      text-align: center;
    }

    nav {
      position: absolute;
      top: 0;
      right: 0;
      padding: 1rem;
    }

    .menu {
      display: none;
      background-color: #fff;
      position: absolute;
      top: 3.5rem;
      right: 1rem;
      border: 1px solid #ccc;
      border-radius: 5px;
      z-index: 999;
    }

    .menu a {
      display: block;
      padding: 10px;
      color: #000;
      text-decoration: none;
    }

    .hamburger {
      font-size: 24px;
      cursor: pointer;
    }

    .dark-mode {
      background-color: #121212;
      color: #f9f9f9;
    }

    .top-left {
      position: absolute;
      top: 1rem;
      left: 1rem;
      display: flex;
      gap: 1rem;
      align-items: center;
    }

    .color-picker label {
      margin-right: 0.5rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Saket Atal ki Rachnayen</h1>
    <p>From the pen of Saket Atal</p>
  </header>

  <div class="top-left">
    <button onclick="toggleTheme()">Light/Dark</button>
    <div class="color-picker">
      <label for="textColor">Text Color:</label>
      <input type="color" id="textColor" onchange="changeTextColor(this.value)" />
    </div>
  </div>

  <nav>
    <span class="hamburger" onclick="toggleMenu()">☰</span>
    <div class="menu" id="menu">
      <a href="index.html">Home</a>
      <a href="urdu-hindi-stories.html">क़लम से: कहानियाँ (Urdu & Hindi Stories)</a>
      <a href="urdu-hindi-poems.html">क़लम से: नज़्में और कविताएं (Urdu & Hindi Poems)</a>
      <a href="english-stories.html">From My Quill: Stories</a>
      <a href="english-poems.html">From My Quill: Poems</a>
      <a href="podcast.html">Podcast - Hind & Hindavi</a>
      <a href="video.html">Video Section - Kissa Jeevan Ka</a>
    </div>
  </nav>

  <script>
    function toggleMenu() {
      const menu = document.getElementById('menu');
      menu.style.display = menu.style.display === 'block' ? 'none' : 'block';
    }

    function toggleTheme() {
      document.body.classList.toggle('dark-mode');
    }

    function changeTextColor(color) {
      document.body.style.color = color;
    }
  </script>
</body>
</html>
