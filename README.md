<!DOCTYPE html><html lang="en"><head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saket Atal's Rachnayen</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: var(--bg);
      color: var(--text);
      transition: background-color 0.3s, color 0.3s;
    }:root {
  --bg: #ffffff;
  --text: #000000;
}

.dark-mode {
  --bg: #121212;
  --text: #ffffff;
}

header {
  padding: 2rem;
  background-color: #333;
  color: white;
  text-align: center;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.5rem 1rem;
  background-color: #444;
  color: white;
}

nav .menu {
  font-size: 1.5rem;
  cursor: pointer;
}

nav .theme-toggle {
  cursor: pointer;
}

.nav-links {
  display: none;
  flex-direction: column;
  background-color: #555;
  padding: 1rem;
}

.nav-links a {
  color: white;
  text-decoration: none;
  margin: 0.5rem 0;
}

footer {
  background: #333;
  color: white;
  padding: 1rem;
  text-align: center;
}

  </style>
</head><body>
  <header>
    <h1>From the Pen of Saket Atal</h1>
    <p>A curated collection of emotions, reflections, and creativity in multiple languages and formats.</p>
  </header>  <nav>
    <div class="menu" onclick="toggleNav()">&#9776;</div>
    <div class="theme-toggle" onclick="toggleTheme()">Toggle Light/Dark</div>
  </nav>
  <div class="nav-links" id="navLinks">
    <a href="kalam-urdu.html">क़लम से - Urdu/Hindi</a>
    <a href="kalam-english.html">Kalam Se - English</a>
    <a href="podcast.html">Hind & Hindavi Podcast</a>
    <a href="video.html">Kissa Jeevan Ka (Video)</a>
  </div>  <footer>
    <p>&copy; 2025 Saket Atal (Dr. Sachin Bhardwaj). All rights reserved.</p>
  </footer>  <script>
    function toggleNav() {
      const navLinks = document.getElementById("navLinks");
      navLinks.style.display = navLinks.style.display === "flex" ? "none" : "flex";
    }

    function toggleTheme() {
      document.body.classList.toggle("dark-mode");
    }
  </script></body></html>
