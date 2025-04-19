<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saket Atal ki Rachnayen</title>
  <!-- Google Fonts Integration -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Raleway:wght@400;600;700&family=Playfair+Display:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary-color: #FF9933;
      --secondary-color: #138808;
      --text-color: #222;
      --background-light: #ffffff;
      --background-dark: #121212;
      --header-font: 'Playfair Display', serif;
      --body-font: 'Raleway', sans-serif;
      --menu-font: 'Poppins', sans-serif;
    }body {
  font-family: var(--body-font);
  margin: 0;
  padding: 0;
  background: linear-gradient(to bottom, var(--primary-color), var(--background-light));
  color: var(--text-color);
  position: relative;
  min-height: 100vh;
  overflow-x: hidden;
}

body::before {
  content: "";
  background-image: url('https://upload.wikimedia.org/wikipedia/commons/5/55/Flag-map_of_India.svg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: 80% auto;
  opacity: 0.12;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: -1;
  pointer-events: none;
}

header {
  background: linear-gradient(135deg, #000080, #000000);
  color: white;
  padding: 2.5rem 2rem;
  text-align: center;
  z-index: 2;
  position: relative;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
  border-bottom: 3px solid var(--primary-color);
}

header h1 {
  font-family: var(--header-font);
  font-size: 3rem;
  margin: 0;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}

header p {
  font-style: italic;
  font-size: 1.3rem;
  margin-top: 0.5rem;
}

nav {
  position: absolute;
  top: 1.5rem;
  right: 1.5rem;
  z-index: 100;
}

.menu {
  display: none;
  background-color: rgba(255, 255, 255, 0.98);
  position: absolute;
  top: 3.5rem;
  right: 0;
  width: 100vw;
  max-width: 500px;
  border-radius: 10px;
  z-index: 3;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
  animation: fadeIn 0.3s ease-in-out;
}

.menu a {
  display: block;
  padding: 16px 24px;
  color: #333;
  text-decoration: none;
  border-bottom: 1px solid rgba(0, 0, 0, 0.05);
  font-family: var(--menu-font);
  font-weight: 600;
  transition: all 0.3s ease;
}

.menu a:hover {
  background-color: rgba(255, 153, 51, 0.2);
  color: var(--primary-color);
}

.hamburger {
  font-size: 30px;
  cursor: pointer;
  background-color: rgba(255, 255, 255, 0.9);
  color: #000080;
  padding: 5px 15px;
  border-radius: 8px;
  box-shadow: 0 3px 8px rgba(0, 0, 0, 0.2);
}

.controls {
  position: fixed;
  bottom: 20px;
  left: 20px;
  background-color: rgba(255, 255, 255, 0.95);
  padding: 12px 16px;
  border-radius: 12px;
  display: flex;
  gap: 1.2rem;
  align-items: center;
  z-index: 4;
}

.controls button {
  background-color: var(--primary-color);
  color: white;
  border: none;
  padding: 8px 15px;
  border-radius: 6px;
  cursor: pointer;
  font-family: var(--body-font);
  font-weight: 600;
}

.controls label {
  font-weight: 500;
}

.controls input[type="color"] {
  border: none;
  width: 35px;
  height: 35px;
  border-radius: 4px;
  cursor: pointer;
}

.main-content {
  padding: 2rem;
  position: relative;
  z-index: 1;
}

  </style>
</head>
<body>
  <header>
    <h1>Saket Atal ki Rachnayen</h1>
    <p>From the pen of Saket Atal</p>
  </header>  <div class="main-content">
    <!-- Your page content will go here -->
  </div>  <div class="controls">
    <button onclick="toggleTheme()">Light/Dark</button>
    <label for="textColor">Text Color:</label>
    <input type="color" id="textColor" onchange="changeTextColor(this.value)" />
    <label for="fontColor">Font Color:</label>
    <input type="color" id="fontColor" onchange="changeFontColor(this.value)" />
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

    function changeFontColor(color) {
      document.querySelectorAll('header h1, header p, .menu a').forEach(el => {
        el.style.color = color;
      });
    }
  </script></body>
</html>
