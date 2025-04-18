<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saket Atal ki Rachnayen</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #FF9933; /* Saffron */
      background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/8/89/India_flag_map.svg/1024px-India_flag_map.svg.png');
      background-repeat: no-repeat;
      background-position: center;
      background-size: 50%;
      color: #222;
      transition: background-color 0.3s, color 0.3s;
    }header {
  background-color: rgba(0, 0, 0, 0.7);
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
  background-color: #fff;
  padding: 5px;
  border-radius: 4px;
}

.dark-mode {
  background-color: #121212;
  color: #f9f9f9;
}

.controls {
  position: fixed;
  bottom: 10px;
  left: 10px;
  background-color: rgba(255, 255, 255, 0.8);
  padding: 10px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
  display: flex;
  gap: 1rem;
  z-index: 1000;
}

.controls label {
  margin-right: 0.5rem;
}

  </style>
</head>
<body>
  <header>
    <h1>Saket Atal ki Rachnayen</h1>
    <p>From the pen of Saket Atal</p>
  </header>  <div class="controls">
    <button onclick="toggleTheme()">Light/Dark</button>
    <label for="textColor">Text Color:</label>
    <input type="color" id="textColor" onchange="changeTextColor(this.value)" />
  </div>  <nav>
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
  </nav>  <script>
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
  </script></body>
</html>
