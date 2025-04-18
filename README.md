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
      background: linear-gradient(to bottom, #FF9933, #ffffff);
      color: #222;
      transition: background-color 0.3s, color 0.3s;
      position: relative;
      min-height: 100vh;
      overflow-x: hidden;
    }body::before {
  content: "";
  background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/8/89/India_flag_map.svg/1024px-India_flag_map.svg.png');
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  opacity: 0.1;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 0;
}

header {
  background-color: rgba(0, 0, 0, 0.8);
  color: white;
  padding: 2rem;
  text-align: center;
  z-index: 2;
  position: relative;
}

header h1 {
  font-size: 2.5rem;
  margin: 0;
}

header p {
  font-style: italic;
  font-size: 1.2rem;
}

nav {
  position: absolute;
  top: 1rem;
  right: 1rem;
  z-index: 3;
}

.menu {
  display: none;
  background-color: #fff;
  position: absolute;
  top: 3rem;
  right: 0;
  border: 1px solid #ccc;
  border-radius: 5px;
  z-index: 3;
}

.menu a {
  display: block;
  padding: 10px 15px;
  color: #000;
  text-decoration: none;
  border-bottom: 1px solid #eee;
}

.menu a:last-child {
  border-bottom: none;
}

.hamburger {
  font-size: 28px;
  cursor: pointer;
  background-color: #fff;
  padding: 5px 10px;
  border-radius: 4px;
  box-shadow: 0 0 6px rgba(0, 0, 0, 0.2);
}

.dark-mode {
  background-color: #121212;
  color: #f9f9f9;
}

.controls {
  position: fixed;
  bottom: 15px;
  left: 15px;
  background-color: rgba(255, 255, 255, 0.9);
  padding: 10px;
  border-radius: 8px;
  display: flex;
  gap: 1rem;
  z-index: 4;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
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
